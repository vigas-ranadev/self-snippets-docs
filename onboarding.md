
SELF ID - Platform Onboarding Doc
===

1. Create an account on https://onboarding.yourself.id/
2. Input your Email and desired Password, submit.
3. On verification screen, input the verification code that you got in your email and submit.
4. Enter Details about you as an platform/attestor, Name, website. Logo/Photo can be skipped for now. 
5. Select a category that your platform falls into, click next.
6. Select "Required for Login" molecules by selecting relevant categories and attestors ( might not be applicable for now as there aren't any attestors )
7. Next step will Ask if you want to generate a new mnemonic or use an existing mnemonic, you can use a funded mnemonic that has already been given to you.
8. It will now register you on the Bitcoin Blockchain using the omni layer protocol. Wait until you get your Transaction ID on screen. Copy all the keys on the screen ( Public Key, Private Key, Public Key Hex, Private Key Hex and Transaction ID ), Click next.
9. After the transaction you will have to wait for about 15 minutes approximately until your transaction is confirmed on the chain and then finally you will have your DID address, which you should be able to see in settings.
10. We can start integrating the frontend code as shown in the onboarding process.
11. Frontend Widget Code 
    ```
    <!-- GOES IN <HEAD> -->
    <script type="text/javascript" src="https://davidshimjs.github.io/qrcodejs/qrcode.min.js"></script>
    <script type="text/javascript" src="https://some-publically-hosted-SELF-ID-address.com/btn.js"></script>
    <link rel="stylesheet" href="https://onboarding.yourself.id/btn.css"
    ```
    ```
    <script>
        // goes in <body>
        createBtn("wss://your-backend-endpoint-wss-enabled.com");
    </script>
    ```
11. Backend code  ( Node.js )
    
    Issue Attestation / Claim
    ---
    ```
    const { issueNewClaim, verifySign } = require("self");

    const claimType = 'general';
    const claimData = { 'general': {name: 'TOM', age: 62 }};
    try {
                        // method imported from SDK
        const issuedClaim = await issueNewClaim({
            blockchain, // omni
            requestorDID,
            claimType,
            claimData,
            attestorName,
            attestorPublicKey: PUBLIC_KEY,
            attestorPrivateKey: PRIVATE_KEY,
            attestorDID: ATTESTOR_DID,
        });
  
    } catch (e) {
        console.log('e :>> ', e);
    }
    ```
    Verify Claim ( Verify the Verifiable Presentation )
    ---
    ```
    const { challenge, token, requestorDID, userVP, clientId } = req.body;
    const { issueNewClaim, verifySign } = require("self");

    const verifyClaim = verifySign(
        JSON.stringify(vc),
        publicKey,
        proof.jws,
        blockchain
    );

    if (verifyClaim) authorizeLogin(clientID);
    ```
    authorizeLogin Method
    --
    ```
    const authorizeLogin = (clientId) => {
    // if client is available, generate a new AccessToken for the
    // client and send needed information to frontend via WebSocket
        wsc[clientId] ?
        wsc[clientId]
            .send(JSON.stringify(
                { 
                    'success': true, 
                    'token': 'xyz' 
                }
            )) :
        console.log("ClientId not found", clientId);
    }

    ```

13. Backend : WebSocket Handling 
    ```
    const wsc = require('../wsc.js')
    wss.on('connection', (ws, req) => {

      var userID = req.url.substr(1);
      console.log('userID :>> ', userID);
      wsc[userID] = ws;
      let randChallenge = Math.random();
      let newAuth = new Auth({ 'challenge': randChallenge });
      newAuth.save();

      //send immediatly a feedback to the incoming connection
      const json = { 
        "endpoint": '/user/handle',
        "challenge": randChallenge,
        "domain": process.env.DOMAIN || 'http://localhost:3000',
        "attestorDID": process.env.ATTESTOR_DID,
        "attestorPublicKeyHex": process.env.PUBLIC_KEY_HEX,
      };
      ws.send(JSON.stringify(json));
    });

    ```
    What is wsc.js?
    ---
    wsc.js is a helpfer file for storing the Active Web Socket connections as it is in an in-memory object. This cannot persist, meaning; once the node.js server is restarted there are no active web sockets.
    ```
    module.exports = {};
    ```
