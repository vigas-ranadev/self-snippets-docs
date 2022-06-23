Oonboarding APP
==
1. [Mnemonic] record charge buyer flush board easily audit daughter enough chat century screen
2. Derived public/private key for bitcoin transaction  
    ```
    {"blockchain": "omni", "bypassDocChecks": true, "didCreator": "mgBr5uvgcCzZDZYB1DbMSKAMPHFx6ZBowF", "didUpdater": "mjNiMif8w8j5LnafNYHVBBM5FMpNjoZXCV", "network": "testnet", "nulldata": "/ipns/16Uiu2HAkvdSRtcGkSE1MZjGirBoE5k8oqssQf3KZgRiKBuFahF7B"}
    ``` 
3. IPFS deterministic keypair for IPNS operation
4. initial call funds the address and next subsequent call to getUtxos fetches
    ```
    {"fee": "0.00000251", "nulldataFee": "0.00000331", "unspents": [{"amount": 0.0002, "desc": "addr(mgBr5uvgcCzZDZYB1DbMSKAMPHFx6ZBowF)#mp257662", "height": 2281900, "rawTx": [Object], "scriptPubKey": "76a914075b0a0ae1a13fc68d5833db04fb6ff85965cecb88ac", "txid": "1fc87bc8a46618ae4d5cb375fbbd94482b692376fa484201f639a59e83c4526d", "vout": 0}]}
    ```
5. ipnsLink 16Uiu2HAkvdSRtcGkSE1MZjGirBoE5k8oqssQf3KZgRiKBuFahF7B embedded in nulldata
6. Data sent for preparing transaction
    ```
    {"didInputs":{"blockchain":"omni","network":"testnet","didCreator":"mgBr5uvgcCzZDZYB1DbMSKAMPHFx6ZBowF","didUpdater":"mjNiMif8w8j5LnafNYHVBBM5FMpNjoZXCV","nulldata":"/ipns/16Uiu2HAkvdSRtcGkSE1MZjGirBoE5k8oqssQf3KZgRiKBuFahF7B","bypassDocChecks":true},"utxos":{"unspents":[{"txid":"1fc87bc8a46618ae4d5cb375fbbd94482b692376fa484201f639a59e83c4526d","vout":0,"scriptPubKey":"76a914075b0a0ae1a13fc68d5833db04fb6ff85965cecb88ac","desc":"addr(mgBr5uvgcCzZDZYB1DbMSKAMPHFx6ZBowF)#mp257662","amount":0.0002,"height":2281900,"rawTx":{"txid":"1fc87bc8a46618ae4d5cb375fbbd94482b692376fa484201f639a59e83c4526d","hash":"1fc87bc8a46618ae4d5cb375fbbd94482b692376fa484201f639a59e83c4526d","version":2,"size":372,"vsize":372,"weight":1488,"locktime":0,"vin":[{"txid":"e8e991054362f305f93df45e2425d6efc0fbf15874e8ca07e8a742973192da5f","vout":12,"scriptSig":{"asm":"30440220147daef98f3b7d8f3c55e696f359ed71b0f53ab46e28101e09694b54f04d63b0022048702dd859ec50ab2403554f0138d2511f590a518fcbdfc53a2682edd0ba7d74[ALL] 024888aff0496d6e720c463edc65655f0a65392921badfea803e642b1aa81ae289","hex":"4730440220147daef98f3b7d8f3c55e696f359ed71b0f53ab46e28101e09694b54f04d63b0022048702dd859ec50ab2403554f0138d2511f590a518fcbdfc53a2682edd0ba7d740121024888aff0496d6e720c463edc65655f0a65392921badfea803e642b1aa81ae289"},"sequence":4294967295},{"txid":"e8e991054362f305f93df45e2425d6efc0fbf15874e8ca07e8a742973192da5f","vout":13,"scriptSig":{"asm":"304402204484b5ade0c8ee076f1d6dd35f83e9a2092ef0f2c73733763b8a46cb1b146dd3022057ffa881c76d8854a59778e002543f7ece9ffe50061a1cf99c6f66a1f04b8562[ALL] 024888aff0496d6e720c463edc65655f0a65392921badfea803e642b1aa81ae289","hex":"47304402204484b5ade0c8ee076f1d6dd35f83e9a2092ef0f2c73733763b8a46cb1b146dd3022057ffa881c76d8854a59778e002543f7ece9ffe50061a1cf99c6f66a1f04b85620121024888aff0496d6e720c463edc65655f0a65392921badfea803e642b1aa81ae289"},"sequence":4294967295}],"vout":[{"value":0.0002,"n":0,"scriptPubKey":{"asm":"OP_DUP OP_HASH160 075b0a0ae1a13fc68d5833db04fb6ff85965cecb OP_EQUALVERIFY OP_CHECKSIG","hex":"76a914075b0a0ae1a13fc68d5833db04fb6ff85965cecb88ac","reqSigs":1,"type":"pubkeyhash","addresses":["mgBr5uvgcCzZDZYB1DbMSKAMPHFx6ZBowF"]}},{"value":0.00014997,"n":1,"scriptPubKey":{"asm":"OP_DUP OP_HASH160 99e7bb4779e7633bb451d6d7ba297ff51e6011ff OP_EQUALVERIFY OP_CHECKSIG","hex":"76a91499e7bb4779e7633bb451d6d7ba297ff51e6011ff88ac","reqSigs":1,"type":"pubkeyhash","addresses":["muYjHPsLerY6wqWoXzP46MVrbwPQsanL6y"]}}],"hex":"02000000025fda92319742a7e807cae87458f1fbc0efd625245ef43df905f362430591e9e80c0000006a4730440220147daef98f3b7d8f3c55e696f359ed71b0f53ab46e28101e09694b54f04d63b0022048702dd859ec50ab2403554f0138d2511f590a518fcbdfc53a2682edd0ba7d740121024888aff0496d6e720c463edc65655f0a65392921badfea803e642b1aa81ae289ffffffff5fda92319742a7e807cae87458f1fbc0efd625245ef43df905f362430591e9e80d0000006a47304402204484b5ade0c8ee076f1d6dd35f83e9a2092ef0f2c73733763b8a46cb1b146dd3022057ffa881c76d8854a59778e002543f7ece9ffe50061a1cf99c6f66a1f04b85620121024888aff0496d6e720c463edc65655f0a65392921badfea803e642b1aa81ae289ffffffff02204e0000000000001976a914075b0a0ae1a13fc68d5833db04fb6ff85965cecb88ac953a0000000000001976a91499e7bb4779e7633bb451d6d7ba297ff51e6011ff88ac00000000","blockhash":"00000000000000d3a6ec2e2e9e2b7781c806102e9e8184a866c0b23c8d416703","confirmations":2,"time":1655969262,"blocktime":1655969262}}],"fee":"0.00000251","nulldataFee":"0.00000331"}}
    ```
7. prepared transaction response
    ```
    70736274ff0100c502000000016d52c4839ea539f6014248fa7623692b4894bdfb75b35c4dae1866a4c87bc81f0000000000ffffffff0322020000000000001976a9142a518aa4d7f7135f1c942be4dec85ae2454cc60488ac0000000000000000456a436f6d6e69000000c82f69706e732f31365569753248416b766453527463476b5345314d5a6a476972426f45356b386f7173735166334b5a6752694b4275466168463742b34a0000000000001976a914075b0a0ae1a13fc68d5833db04fb6ff85965cecb88ac00000000000100fd740102000000025fda92319742a7e807cae87458f1fbc0efd625245ef43df905f362430591e9e80c0000006a4730440220147daef98f3b7d8f3c55e696f359ed71b0f53ab46e28101e09694b54f04d63b0022048702dd859ec50ab2403554f0138d2511f590a518fcbdfc53a2682edd0ba7d740121024888aff0496d6e720c463edc65655f0a65392921badfea803e642b1aa81ae289ffffffff5fda92319742a7e807cae87458f1fbc0efd625245ef43df905f362430591e9e80d0000006a47304402204484b5ade0c8ee076f1d6dd35f83e9a2092ef0f2c73733763b8a46cb1b146dd3022057ffa881c76d8854a59778e002543f7ece9ffe50061a1cf99c6f66a1f04b85620121024888aff0496d6e720c463edc65655f0a65392921badfea803e642b1aa81ae289ffffffff02204e0000000000001976a914075b0a0ae1a13fc68d5833db04fb6ff85965cecb88ac953a0000000000001976a91499e7bb4779e7633bb451d6d7ba297ff51e6011ff88ac0000000000000000
    ```
8. Signed transaction
    ```
    {"data": "02000000016d52c4839ea539f6014248fa7623692b4894bdfb75b35c4dae1866a4c87bc81f000000006a473044022074f50f9bd2f3a8f6e7975fdc16a2160f7d0822a8ff279681b2359af489c0ccd202203cfa9176f14e0af41c7452fcd3a0ead6b06bd57f420c21e957a4336a05af74500121035c082f07af9d14cabfbac9aef00a921ecd124e0dff1d91a8000c265ed2dad7c6ffffffff0322020000000000001976a9142a518aa4d7f7135f1c942be4dec85ae2454cc60488ac0000000000000000456a436f6d6e69000000c82f69706e732f31365569753248416b766453527463476b5345314d5a6a476972426f45356b386f7173735166334b5a6752694b4275466168463742b34a0000000000001976a914075b0a0ae1a13fc68d5833db04fb6ff85965cecb88ac00000000", "success": true}
    ```
9. broadcasted transaction
    ```
    10cbb298828af92e737f063b1e811e1e7347dcf8fa93b4236e5d09ab6f805d47
    ```
10. on confirmation tx ... encoded in DID format 
    ```
        "did": "did:mdip:omni-xu6g-tyyq-qrwn-pdg"
    ```

Netki Flow
===
1. just like above flow netki will create their DID and would look something like this
    ```
    {
    "@context": [
        "https://www.w3.org/ns/did/v1"
    ],
    "publicKey": [
        {
            "id": "#auth",
            "type": "EcdsaSecp256k1VerificationKey2019",
            "publicKeyBase58": "myV7KfUG7xsnaU9BBpeNPBjMSiJF4oE5ad"
        },
        {
            "id": "#vc-pubkey",
            "type": "EcdsaSecp256k1VerificationKey2019",
            "publicKeyBase58": "myV7KfUG7xsnaU9BBpeNPBjMSiJF4oE5ad"
        }
    ],
    "authentication": [
        "#auth"
    ],
    "assertionMethod": [
        "#vc-pubkey"
    ],
    "updatedAt": 1654761657349,
    "tsProperty": 1654761596956,
    "id": "did:mdip:omni-xs6n-fy2p-qx5z-4ty",
    "platform": {
        "molecules": [],
        "_id": "62a1a400682342222f4f1a23",
        "userId": "62a1a3e11fe0672168ff7212",
        "__v": 0,
        "categoryId": "6107de499d0e7d106c5a9279",
        "createdAt": "2022-06-09T07:40:48.780Z",
        "name": "Netki Inc",
        "updatedAt": "2022-06-09T07:40:48.780Z",
        "category": {
            "_id": "6107de499d0e7d106c5a9279",
            "name": "Business",
            "createdAt": "2022-06-09T07:40:29.184Z"
        },
        "website": "netki.com"
    }
    }
    ```

2. Netki app creates new authentication session with its backend, with reference client ID say `53cf67c2-e41e`
3. Netki opens SELF app and passes the session data to SELF app for a new authorization request, no molecules are asked as there is no `required for login` in the DID document.
    ```
    {"attestorDID": "did:mdip:omni-xs6n-fy2p-qx5z-4ty", "attestorIPFS": "/ipfs/QmZy1W9P7QVZPbCsWGHTs9gezUJzzvckD1v7wSCWqZaP9q", "attestorIPNS": "/ipns/16Uiu2HAkyMuaCohK1zh8x5wEuKKTG55LWibi1GmKHWr4pRfu69wx", "attestorName": "Netki", "attestorPublicKeyHex": "038d6478c9f1dd73239d1f670d86cb2a28c1bbb2d09502131d30059bcb6c1e4758", "challenge": "0.9090484880926222", "clientId": "53cf67c2-e41e", "domain": "verix-attestor-backend.byrana.xyz", "endpoint": "/self/user"}
    ```
4. On request, SELF fetches the details from the DID doc and presents it on the screen for approval
    ```
    {"@context": ["https://www.w3.org/ns/did/v1"], "assertionMethod": ["#vc-pubkey"], "authentication": ["#auth"], "id": "did:mdip:omni-xs6n-fy2p-qx5z-4ty", "platform": {"__v": 0, "_id": "62a1a400682342222f4f1a23", "category": {"_id": "6107de499d0e7d106c5a9279", "createdAt": "2022-06-09T07:40:29.184Z", "name": "Business"}, "categoryId": "6107de499d0e7d106c5a9279", "createdAt": "2022-06-09T07:40:48.780Z", "molecules": [], "name": "Netki Inc", "updatedAt": "2022-06-09T07:40:48.780Z", "userId": "62a1a3e11fe0672168ff7212", "website": "netki.com"}, "publicKey": [{"id": "#auth", "publicKeyBase58": "myV7KfUG7xsnaU9BBpeNPBjMSiJF4oE5ad", "type": "EcdsaSecp256k1VerificationKey2019"}, {"id": "#vc-pubkey", "publicKeyBase58": "myV7KfUG7xsnaU9BBpeNPBjMSiJF4oE5ad", "type": "EcdsaSecp256k1VerificationKey2019"}], "tsProperty": 1654761596956, "updatedAt": 1654761657349}
    ```    
5. On approval, as SELF do not have a VC from netki, so SELF app asks netki backend for a signup, once signed up, we have a VC with no user data 
6. Netki backend allows this signup and makes a new VC
    ```
    {"@context": ["https://www.w3.org/2018/credentials/v1"], "credentialSubject": {"general": {"loggedIn": true}, "id": "did:mdip:omni-xu6g-tyyq-qrwn-pdg"}, "expirationDate": "2022-12-20T07:56:24.840Z", "id": "did:mdip:omni-xs6n-fy2p-qx5z-4ty", "issuanceDate": "2022-06-23T07:56:24.840Z", "issuer": {"id": "did:mdip:omni-xs6n-fy2p-qx5z-4ty", "name": "Netki"}, "proof": {"created": "2022-06-23T07:56:24.840Z", "jws": "H/5/oe5adZS8B1vALLh8yGeQDxq7Z+unZzTM3slQVYtPeqwRfhDWOnwzdeaSuaXVjNWvsLO9b49hc5MnVme1FGQ=", "proofPurpose": "assertionMethod", "type": "EcdsaSecp256k1VerificationKey2019", "verificationMethod": "n4oR9sWqwixDFPUew8gy2MFWCT2QJXTPNR"}, "type": ["VerifiableCredential", "general"]}
    ```
7. this VC is now encrypted using public key hash `035c082f07af9d14cabfbac9aef00a921ecd124e0dff1d91a8000c265ed2dad7c6` and uploads it on IPFS and CID is `QmW7NqgvVPjQEDfeRKrKoh2Rv3eVPhn9XPgH1S23yKckLK`
8. SELF app gets this CID in the HTTP request for signup to netki backend
9. SELF app, resolves the CID, decrypts the data using private key derived from HD wallet. Saves the VC to redux/storage in app.
10. In next subsequent call to netki for login, SELF app knows it has a VC from netki, makes VP
    ```
    {"@context": ["https://www.w3.org/2018/credentials/v1"], "proof": {"challenge": "0.9090484880926222", "created": "2022-06-23T07:56:31.065Z", "domain": "verix-attestor-backend.byrana.xyz", "jws": "H5xRTC62pKTb2645fth/jSuOsYsq5oCFNzwHfhCVKudDDWXWIQdFILJrYxb3Ye8v7kD2CGYa6nc72oDcYaQN3QU=", "proofPurpose": "authentication", "type": "EcdsaSecp256k1VerificationKey2019", "verificationMethod": "mgBr5uvgcCzZDZYB1DbMSKAMPHFx6ZBowF"}, "type": "VerifiablePresentation", "verifiableCredential": [{"@context": [Array], "credentialSubject": [Object], "expirationDate": "2022-12-20T07:56:24.840Z", "id": "did:mdip:omni-xs6n-fy2p-qx5z-4ty", "issuanceDate": "2022-06-23T07:56:24.840Z", "issuer": [Object], "proof": [Object], "type": [Array]}]}
    ```
11. SELF app now Encrypts VP,  uploads to IPFS and gets CID `QmTLeQSHuSWTwzV3vCC7LDZMR7vyybhWRAsWpU3VzAoiqf` and sends this data to netki's backend
    ```
    {"challenge": "0.9090484880926222", "clientId": "53cf67c2-e41e", "publicKey": "035c082f07af9d14cabfbac9aef00a921ecd124e0dff1d91a8000c265ed2dad7c6", "requestorDID": "did:mdip:omni-xu6g-tyyq-qrwn-pdg", "token": "abc", "userVP": "QmTLeQSHuSWTwzV3vCC7LDZMR7vyybhWRAsWpU3VzAoiqf"}
    ```
12. Netki Backend sees a userVP being sent and figures it's trying to login, so netki, fetches this IPFS doc, decrypts it and verifies the VP to make sure it was issued by netki itself, allows login.
13. At this point user in self app sees a message - login success, please go back to netki app.
14. User opens netki app, netki app checks if the login for client id `53cf67c2-e41e` is authorized? awesome. Let this client log in, send needed Tokens everything.
15. Netki app is now logged in , user does SCAN, Netki's backend awaits the data to be available from actual netki's servers. When data is available, data is presented to netki user to make sure the data is right, on confirmation :: all these data atoms are sent as attestation to the DID address using an endpoint deployed by SELF
    ```
    var axios = require('axios');
    var data = JSON.stringify({
    "did": "did:mdip:omni-xu6g-tyyq-qrwn-pdg",
    "cid": "cidOfIPFS"
    });

    var config = {
    method: 'post',
    url: 'self-marketplace-api-hourly.byrana.xyz/api/attestor/offloadAttestation',
    headers: { 
        'Authorization': 'Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYyOWRhOTBlMWZlMDY3MjE2OGZmNzFlZSIsImlhdCI6MTY1NDYxMTIyMCwiZXhwIjozMzE0NDA2NDQwfQ.gHyrFMAvnSUlIaonN5MNbHfR6jnUM4KP9Ts3PUBDop0', 
        'Content-Type': 'application/json'
    },
    data : data
    };

    axios(config)
    .then(function (response) {
    console.log(JSON.stringify(response.data));
    })
    .catch(function (error) {
    console.log(error);
    });
        ```
16. user goes back to SELF app. SELF app keeps checking time to time if there are any new attestation CID available at SELF's endpoint for his DID
    ```
    var axios = require('axios');
    var data = '';

    var config = {
    method: 'get',
    url: 'self-marketplace-api-hourly.byrana.xyz/api/attestor/fetchAttestations/did:mdip:omni-xu6g-tyyq-qrwn-pdg/',
    headers: { },
    data : data
    };

    axios(config)
    .then(function (response) {
    console.log(JSON.stringify(response.data));
    })
    .catch(function (error) {
    console.log(error);
    });
    ```
17. when any new attestation is available, it is fetched from IPFS using CID, decrypted and saved to redux store of SELF APP ( locally )

