# Public VeChain Thor nodes

VeBlocks provides access to all VeChain Thor networks via publicly accessible HTTP/HTTPS connections. This is a community project to support all developers and allow them everywhere-access to the blockchain, without the need to have a full node with them.
I will not collect or chance any data coming/going to the nodes. There are just some logs kept for maintenance and performance evaluation. These logs will be deleted after 14 days. 

## Getting Started

All node are maintained by VeBlocks and always kept compatible with the networks. The only limitation is 3000 open connections per IP address. The nodes are accessible via HTTP/HTTPS and P2P, making them also available as bootnode.


## Using the nodes

### Use nodes in Sync
Use the following node endpoints:   
Mainnet: https://sync-mainnet.veblocks.net   
Testnet: https://sync-testnet.veblocks.net   


Demo HowTo: https://youtu.be/FogF2c-ypSg
   


### VeChain mainnet node
```
Cloudflare, loadbalanced:
https://mainnet.veblocks.net
wss://mainnet.veblocks.net/subscriptions/beat

Direct access (no cloudflare):
http://mainnet.vechain.blockorder.net
https://mainnet.vechain.blockorder.net
```

### VeChain testnet node
```
Cloudflare, loadbalanced:
https://testnet.veblocks.net 
wss://testnet.veblocks.net/subscriptions/beat

Direct access (no cloudflare):
http://testnet.vechain.blockorder.net
https://testnet.vechain.blockorder.net
```


### VeChain solo node
```
Cloudflare:
https://solo.veblocks.net
wss://solo.veblocks.net/subscriptions/beat

```
(resets all 24 hours)

These addresses cointain VET/VTHO in SOLO:


| Address        | Mnemonic|
| :------------- |:-----------|
 0xf077b491b355E64048cE21E3A6Fc4751eEeA77fa| denial kitchen pet squirrel other broom bar gas better priority spoil cross 



### Example use


Get best block: 
```
curl -X GET "https://mainnet.veblocks.net/blocks/best" -H  "accept: application/json"
```


Get BlockRef:
```
curl -s -X GET https://mainnet.veblocks.net/blocks/best -H  "accept: application/json" | jq -r .id | cut -c-18
```

Use as bootnode:
```
./thor --network main --bootnode enode://6bd860159b853d76d77a850f20e5975bb784756058cf8d32ea6f79eeb40b73e4dda5fbc05a6ca2764df2cd119f548b30162fcc9df63e956a8dd09923e712c1a6@95.216.240.98:11235
```
   

### Uptime and connectivity
This is a community project and the nodes will be up as much as possible but there may be short downtimes due to updates/upgrades or any other hard/software failure. VeBlocks is not responsible for your software. Consider these variables when using the nodes!

### Pre-compiled windows nodes
You can use my precompiled windows thor node software. This will use up about 60GB on your C-drive and will take 8-48h to sync. Always remember that this is a "quality of life"-download. If you want to use thor in a professional environment, compile the software yourself to ensure data-integrity.

https://cdn.veblocks.net/VeChain-thor1.6.0.zip

## Contact
E-Mail: veblocks@pm.me  
Telegram: https://t.me/mirei83   
Donation: 0xD88bf449EcF41993685fDA562FBB23a5fE7fFCd5 (VeChain)

