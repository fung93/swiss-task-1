# SWISSTRONIK Technical Task 1

Steps to deploy smart contract using hardhat

1. Create new repository
```shell
https://github.com/fung93/swiss-task-1.git
```
2. Install hardhat
```shell
npm install --save-dev hardhat
```
```shell
npm install --save-dev @nomicfoundation/hardhat-toolbox
```
```shell
npx hardhat
```
3. Import Private Key start with 0x
```shell
require("@nomicfoundation/hardhat-toolbox");

module.exports = {
  solidity: "0.8.19",
  networks: {
    swisstronik: {
      url: "https://json-rpc.testnet.swisstronik.com/",
      accounts: ["0xd5..."], //Your private key starting with "0x"
    },
  },
};
```
4. Compile contract file
```shell
npx hardhat compile
```
5. Deploy contract
```shell
npx hardhat run scripts/deploy.js --network swisstronik
```
By : 
github : fung93
twitter : @ffffung93
