# Forking Mainnet Ethereum Chain | Testing Localhost with Laika

## Install the Dependencies and Dotenv

```shell
yarn install
```

```shell
yarn install dotenv
```

## Create .env file

```shell
RPC_URL = ""
PRIVATE_KEY = ""
ETHERSCAN_API= ""

RPC_URL_FORK = "http://localhost:8545"
PRIVATE_KEY_FORK = ""
```
## Forking Ethereum Mainnet with Alchemy

```shell
npx hardhat node --fork https://eth-mainnet.g.alchemy.com/v2/<API_ALCHEMY_KEY>
```

## Compiling the Smart Contracts

```shell
npx hardhat compile
```

## Deploy Smart Contracts on Ethereum Fork

```shell
npx hardhat run --network fork scripts/deploy.js
```

## Login in Laika with your Metamask Account

https://web.getlaika.app/

## Sync Deployed Smart Contract with Laika

```shell
npx hardhat laika-sync --contract <contract_name> --address <OPTIONAL address_of_that_contract>
```
