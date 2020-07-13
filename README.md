# Public VeChain Thor nodes

VeBlocks provides access to all VeChain Thor networks via publicly accessible HTTP/HTTPS connections. This is a community project to support all developers and allow them everywhere-access to the blockchain, without the need to have a full node with them.

## Getting Started

All node are maintained by VeBlocks and always kept compatible with the networks. The only limitation is 3000 open connections per IP address. The nodes are accessible via HTTP/HTTPS and P2P, making them also availible as bootnode.


## Using the nodes

### VeChain mainnet node
```
HTTP:   http://mainnet.veblocks.net
HTTPS:  https://mainnet.veblocks.net
P2P:    enode://6bd860159b853d76d77a850f20e5975bb784756058cf8d32ea6f79eeb40b73e4dda5fbc05a6ca2764df2cd119f548b30162fcc9df63e956a8dd09923e712c1a6@95.216.240.98:11235
```

### VeChain testnet node
```
HTTP:   http://testnet.veblocks.net
HTTPS:  https://testnet.veblocks.net
P2P:    enode://04bbc1fd670fb4fa56eaa44978c8bb0acd5542c6f4460d732ecba2ad9c8aac3ca90513588a3a432af0c93ceb614d86e6db4ac866a9f74a55a9358602f6bf658a@95.216.240.99:11235
```

### VeChain solo node
```
HTTP:   http://solo.veblocks.net
HTTPS:  https://solo.veblocks.net
```
(resets all 24 hours)

### Example use


Get best block: 
```
curl -X GET "https://mainnet.veblocks.net/blocks/best" -H  "accept: application/json"
```


Get BlockRef:
```
curl -s -X GET https://mainnet.veblocks.net/blocks/best -H  "accept: application/json" | jq -r .id | cut -c-18
```


### Uptime and connectivity
This is a community project and the nodes will be up as much as possible but there may be short downtimes due to updates/upgrades or any other hard/software failure. VeBlocks is not responsible for your software. Consider these variables when using the nodes!

## Contact
E-Mail: veblocks@pm.me  
Telegram: https://t.me/mirei83

