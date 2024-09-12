## Auto Transfer BOT
### Faucet:
1. Movement MEVM:
   [Link](https://faucet.movementlabs.xyz/?network=mevm)
2. Sonic Fantom Testnet:
   [Link](https://testnet.soniclabs.com/account)
3. Plume Testnet:
   [Link]()
4. Story Testnet:
   [Link](https://faucet.story.foundation/)
5. Minato:
    [Link](https://bridge.soneium.org/en/testnet)
6. Swisstronik Testnet:
    [Link](https://faucet.testnet.swisstronik.com/)
7. Hemi Testnet:
    [Link](https://app.hemi.xyz/en/tunnel/)
8. Curtis:
    [Link](https://curtis.hub.caldera.xyz/)

### Installation
1. Clone the repository:
```bash
git clone https://github.com/dante4rt/evm-auto-transfer.git
cd evm-auto-transfer
```
2. Install the necessary packages:
```bash
npm install
```
### Configuration
1. Define the Chains:
```bash
rm /chains/testnet.json && nano /chains/testnet.json
```
   Edit new `testnet.json` with below code.

```Bash
[
  {
    "name": "Movement MEVM",
    "rpcUrl": "https://mevm.devnet.imola.movementlabs.xyz",
    "chainId": "30732",
    "symbol": "MOVE",
    "explorer": "https://explorer.devnet.imola.movementlabs.xyz"
  },
  {
    "name": "Sonic Fantom Testnet",
    "rpcUrl": "https://rpc.testnet.soniclabs.com",
    "chainId": "64165",
    "symbol": "S",
    "explorer": "https://testnet.soniclabs.com"
  },
  {
    "name": "Plume Testnet",
    "rpcUrl": "https://testnet-rpc.plumenetwork.xyz/http",
    "chainId": "161221135",
    "symbol": "ETH",
    "explorer": "https://testnet-explorer.plumenetwork.xyz"
  },
  {
    "name": "Story Testnet",
    "rpcUrl": "https://testnet.storyrpc.io",
    "chainId": "1513",
    "symbol": "IP",
    "explorer": "https://testnet.storyscan.xyz"
  },
  {
    "name": "Minato",
    "rpcUrl": "https://rpc.minato.soneium.org/",
    "chainId": "1946",
    "symbol": "ETH",
    "explorer": "https://explorer-testnet.soneium.org"
  },
  {
    "name": "Swisstronik Testnet",
    "rpcUrl": "https://json-rpc.testnet.swisstronik.com/",
    "chainId": "1291",
    "symbol": "SWTR",
    "explorer": "https://explorer-evm.testnet.swisstronik.com/"
  },
  {
    "name": "Hemi Testnet",
    "rpcUrl": "https://testnet.rpc.hemi.network/rpc",
    "chainId": "743111",
    "symbol": "ETH",
    "explorer": "https://testnet.explorer.hemi.xyz"
  },
  {
    "name": "Curtis",
    "rpcUrl": "https://curtis.rpc.caldera.xyz/http",
    "chainId": "33111",
    "symbol": "APE",
    "explorer": "https://curtis.explorer.caldera.xyz"
  }
]
```
2. Define Private Key:
```Bash
nano privateKeys.json
```
     ```json
     [
         "0xYOUR_PRIVATE_KEY_1"
     ]
     ```
### Run Transfer BOT
1. Run the script for random address generation and transactions:
```bash
npm start
```
Check your transactions on Explorer!
