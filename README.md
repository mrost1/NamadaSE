# NamadaSE
Namada tasks

Operating IBC / Interoperability infrastructure
Cosmos (theta-testnet-001) - Namada SE (shielded-expedition.88f17d1d14) 

Command on Cosmos:

gaiad tx ibc-transfer transfer transfer channel-3828 tnam1qplcsk0hxncxxfvun4vxqrk0s9p37cr70gkul7et 1000uatom --from cosmos1x4q0t35vvsv4qtzxhxsfa62ucdjzd8vy4k8fv8 --fees 5000uatom

txhash: 6E15F62DE5978AC284AA7DDBE9F75601CC9995A021D34FE77139DC5528F13362

namadac balance --owner  relayer --node http://localhost:26657
naan: 713.5
transfer/channel-311/uatom: 1000

On block explorer (proof):
https://www.mintscan.io/cosmoshub-testnet/tx/92BEFE13863D591EC5383E1B685362C6F18AF5C2639C4C3DF6BF529E497A21E6?height=20438105 

Command on Namada:

namadac ibc-transfer --source relayer --receiver cosmos1x4q0t35vvsv4qtzxhxsfa62ucdjzd8vy4k8fv8 --token naan  --amount 100 --channel-id channel-311  --memo tpknam1qpall8pt60ek5zgeyxstdkhrp34rrqj67a2jrklrl9sddln0grq87nluum5 --node http://localhost:26657
Transaction added to mempool.
Wrapper transaction hash: 5A18C2ED74B67A2038EFC5072B5923334D362EE19C6FC9CEACEF957DF16D410C
Inner transaction hash: AE661A9B50CF42432EB5C0DBDDCF387978D4FFC87AAA81B3D908FB0FF92EEF0A
Wrapper transaction accepted at height 55159. Used 26 gas.
Waiting for inner transaction result...
Transaction was successfully applied at height 55160. Used 6193 gas.

gaiad query bank balances  cosmos1x4q0t35vvsv4qtzxhxsfa62ucdjzd8vy4k8fv8
balances:
- amount: "100"
  denom: ibc/04B45BC164F984517C1403BF8A92D50E19FF8EB75A1411F9AC024B65136DEBD4
- amount: "2887683"
  denom: uatom



