# Supply chain & data auditing

This repository containts an Ethereum DApp that demonstrates a Supply Chain flow between a Seller and Buyer. The user story is similar to any commonly used supply chain process. A Seller can add items to the inventory system stored in the blockchain. A Buyer can purchase such items from the inventory system. Additionally a Seller can mark an item as Shipped, and similarly a Buyer can mark an item as Received.

The DApp User Interface when running should look like...

![truffle test](images/ftc_product_overview.png)

![truffle test](images/ftc_farm_details.png)

![truffle test](images/ftc_product_details.png)

![truffle test](images/ftc_transaction_history.png)


## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

Please make sure you've already installed ganache-cli, Truffle and enabled MetaMask extension in your browser.

```
Give examples (to be clarified)
```

### Installing

> The starter code is written for **Solidity v0.4.24**. At the time of writing, the current Truffle v5 comes with Solidity v0.5 that requires function *mutability* and *visibility* to be specified (please refer to Solidity [documentation](https://docs.soliditylang.org/en/v0.5.0/050-breaking-changes.html) for more details). To use this starter code, please run `npm i -g truffle@4.1.14` to install Truffle v4 with Solidity v0.4.24. 

A step by step series of examples that tell you have to get a development env running

Clone this repository:

```
git clone https://github.com/udacity/nd1309/tree/master/course-5/project-6
```

Change directory to ```project-6``` folder and install all requisite npm packages (as listed in ```package.json```):

```
cd project-6
npm install
```

Launch Ganache:

```
ganache-cli -m "spirit supply whale amount human item harsh scare congress discover talent hamster"
```

Your terminal should look something like this:

![truffle test](images/ganache-cli.png)

In a separate terminal window, Compile smart contracts:

```
truffle compile
```

Your terminal should look something like this:

![truffle test](images/truffle_compile.png)

This will create the smart contract artifacts in folder ```build\contracts```.

Migrate smart contracts to the locally running blockchain, ganache-cli:

```
truffle migrate
```

Your terminal should look something like this:

![truffle test](images/truffle_migrate.png)

Test smart contracts:

```
truffle test
```

All 10 tests should pass.

![truffle test](images/truffle_test.png)

In a separate terminal window, launch the DApp:

```
npm run dev
```

## Built With

* [Ethereum](https://www.ethereum.org/) - Ethereum is a decentralized platform that runs smart contracts
* [IPFS](https://ipfs.io/) - IPFS is the Distributed Web | A peer-to-peer hypermedia protocol
to make the web faster, safer, and more open.
* [Truffle Framework](http://truffleframework.com/) - Truffle is the most popular development framework for Ethereum with a mission to make your life a whole lot easier.


## Authors

See also the list of [contributors](https://github.com/your/project/contributors.md) who participated in this project.

## Acknowledgments

* Solidity
* Ganache-cli
* Truffle
* IPFS

## Contract deployed
Starting migrations...
======================
> Network name:    'rinkeby'
> Network id:      4
> Block gas limit: 29970705 (0x1c95111)


1_initial_migration.js
======================

   Deploying 'Migrations'
   ----------------------
   > transaction hash:    0x5c3e768f51470fa9f6011ec6bc9e60de74e2cf0b4ff504783d5ebe9c0a38d1c0
   > Blocks: 2            Seconds: 17
   > contract address:    0xc8623b1C5CD0F89d34C6e989Cb5891Bc03BcBf27
   > block number:        10204590
   > block timestamp:     1645414611
   > account:             0x3a59B9d754c7DBF49fe2617Aab2Dc73764d97d56
   > balance:             0.046363264962545507
   > gas used:            226537 (0x374e9)
   > gas price:           1.000000022 gwei
   > value sent:          0 ETH
   > total cost:          0.000226537004983814 ETH


   > Saving migration to chain.
   > Saving artifacts
   -------------------------------------
   > Total cost:     0.000226537004983814 ETH


2_deploy_contracts.js
=====================

   Deploying 'FarmerRole'
   ----------------------
   > transaction hash:    0x9214296adeb64fef97a4ba123b86c3c57c7414b523da5a964351217519a61cb2
   > Blocks: 2            Seconds: 21
   > contract address:    0x6eb6Bc00D8B7cD655D9D6b9ce94aaE0B96B94a6A
   > block number:        10204593
   > block timestamp:     1645414656
   > account:             0x3a59B9d754c7DBF49fe2617Aab2Dc73764d97d56
   > balance:             0.045988575954631275
   > gas used:            328926 (0x504de)
   > gas price:           1.000000021 gwei
   > value sent:          0 ETH
   > total cost:          0.000328926006907446 ETH


   Deploying 'DistributorRole'
   ---------------------------
   > transaction hash:    0xb5576bce96c27468c3d6f4c0a8ade8b46b222deb2269b1bd1e77d8f2cc1ee034
   > Blocks: 2            Seconds: 17
   > contract address:    0x1Fcc5b0C7C5167a27D06D4559B150cAB0806C164
   > block number:        10204595
   > block timestamp:     1645414686
   > account:             0x3a59B9d754c7DBF49fe2617Aab2Dc73764d97d56
   > balance:             0.045659601948051795
   > gas used:            328974 (0x5050e)
   > gas price:           1.00000002 gwei
   > value sent:          0 ETH
   > total cost:          0.00032897400657948 ETH


   Deploying 'RetailerRole'
   ------------------------
   > transaction hash:    0xbbc75e922b1efca37807e5919bb17a238c02798f6e26d5f5dc49590feaa92d31
   > Blocks: 2            Seconds: 21
   > contract address:    0xC92B9dF10aA6cA6Cd8b96Cf2BfD5307eC064996e
   > block number:        10204597
   > block timestamp:     1645414716
   > account:             0x3a59B9d754c7DBF49fe2617Aab2Dc73764d97d56
   > balance:             0.045330651942130695
   > gas used:            328950 (0x504f6)
   > gas price:           1.000000018 gwei
   > value sent:          0 ETH
   > total cost:          0.0003289500059211 ETH


   Deploying 'ConsumerRole'
   ------------------------
   > transaction hash:    0x508a83aaf855a52aba3c47bd4ecb9877792b77fe1c839cfad3d80817b2225071
   > Blocks: 2            Seconds: 21
   > contract address:    0x363D2a9e24cFca4694A75dF2Dbf680Aadb63d074
   > block number:        10204599
   > block timestamp:     1645414746
   > account:             0x3a59B9d754c7DBF49fe2617Aab2Dc73764d97d56
   > balance:             0.045001701936867495
   > gas used:            328950 (0x504f6)
   > gas price:           1.000000016 gwei
   > value sent:          0 ETH
   > total cost:          0.0003289500052632 ETH


   Deploying 'SupplyChain'
   -----------------------
   > transaction hash:    0xb88e581f4809da33564fc3e7a266a31cd4490d7fa9a26ea66a523bd73ac13667
   > Blocks: 2            Seconds: 21
   > contract address:    0x4Eb577480BeF7420Be1929107D3B0F8434C1E943
   > block number:        10204601
   > block timestamp:     1645414776
   > account:             0x3a59B9d754c7DBF49fe2617Aab2Dc73764d97d56
   > balance:             0.041832233889325475
   > gas used:            3169468 (0x305cbc)
   > gas price:           1.000000015 gwei
   > value sent:          0 ETH
   > total cost:          0.00316946804754202 ETH


   > Saving migration to chain.
   > Saving artifacts
   -------------------------------------
   > Total cost:     0.004485268072213246 ETH


Summary
=======
> Total deployments:   6
> Final cost:          0.00471180507719706 ETH