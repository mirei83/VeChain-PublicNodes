# Public VeChain Thor nodes

VeBlocks provides access to all VeChain Thor networks via publicly accessible HTTP/HTTPS connections. This is a community project to support all developers and allow them everywhere-access to the blockchain, without the need to have a full node with them.

## Getting Started

All node are maintained by VeBlocks and always kept compatible with the networks. The only limitation is 3000 open connections per IP address. The nodes are accessible via HTTP/HTTPS and P2P, making them also available as bootnode.


## Using the nodes

### VeChain mainnet node
```
http://mainnet.veblocks.net
https://mainnet.veblocks.net
ws://mainnet.veblocks.net/subscriptions/beat
wss://mainnet.veblocks.net/subscriptions/beat
P2P:    enode://6bd860159b853d76d77a850f20e5975bb784756058cf8d32ea6f79eeb40b73e4dda5fbc05a6ca2764df2cd119f548b30162fcc9df63e956a8dd09923e712c1a6@95.216.240.98:11235
```

### VeChain testnet node
```
http://testnet.veblocks.net
https://testnet.veblocks.net
ws://testnet.veblocks.net/subscriptions/beat
wss://testnet.veblocks.net/subscriptions/beat
P2P:    enode://04bbc1fd670fb4fa56eaa44978c8bb0acd5542c6f4460d732ecba2ad9c8aac3ca90513588a3a432af0c93ceb614d86e6db4ac866a9f74a55a9358602f6bf658a@95.216.240.99:11235
```

### VeChain solo node
```
http://solo.veblocks.net
https://solo.veblocks.net
ws://solo.veblocks.net/subscriptions/beat
wss://solo.veblocks.net/subscriptions/beat
```
(resets all 24 hours)

These addresses cointain VET/VTHO in SOLO:


| Address        | Private Key|
| :------------- |:-----------|
 0x7567d83b7b8d80addcb281a71d54fc7b3364ffed| dce1443bd2ef0c2631adc1c67e5c93f13dc23a41c18b536effbbdcbcdb96fb65 
 0xd3ae78222beadb038203be21ed5ce7c9b1bff602| 321d6443bc6177273b5abf54210fe806d451d6b7973bccc2384ef78bbcd0bf51 
 0x733b7269443c70de16bbf9b0615307884bcc5636| 2d7c882bad2a01105e36dda3646693bc1aaaa45b0ed63fb0ce23c060294f3af2 
 0x115eabb4f62973d0dba138ab7df5c0375ec87256| 593537225b037191d322c3b1df585fb1e5100811b71a6f7fc7e29cca1333483e 
 0x199b836d8a57365baccd4f371c1fabb7be77d389| ca7b25fc980c759df5f3ce17a3d881d6e19a38e651fc4315fc08917edab41058 
 0x5e4efedf3d71232340280d8bc475421352994b63| 88d2d80b12b92feaa0da6d62309463d20408157723f2d7e799b6a74ead9a673b 
 0x29f72dc07224a4c6270407bfd6b8fec559d29f6c| fbb9e7ba5fe9969a71c6599052237b91adeb1e5fc0c96727b66e56ff5d02f9d0 
 0x47109a193c49862c89bd76fe2de3585743dd2bb0| 547fb081e73dc2e22b4aae5c60e2970b008ac4fc3073aebc27d41ace9c4f53e9 
 0xa5e255d4c65af201b97210ff4cd9521a46427654| c8c53657e41a8d669349fc287f57457bd746cb1fcfc38cf94d235deb2cfca81b 
 0x0489a3fff1930b85f1d73eff8a4699281aadb558| 87e0eba9c86c494d98353800571089f316740b0cb84c9a7cdf2fe5c9997c7966 



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

https://cdn.veblocks.net/VeChain-thor1.3.6.zip

## Contact
E-Mail: veblocks@pm.me  
Telegram: https://t.me/mirei83   
Donation: 0xD88bf449EcF41993685fDA562FBB23a5fE7fFCd5 (VeChain)

