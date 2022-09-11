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


## Deployment Information 

### Rinkeby network

```
Deploying 'FarmerRole'
   ----------------------
   > transaction hash:    0xe9ca1fc5883b03ae6e7b6d75e7ef3f43d65ecf4738cc520630fadc240b3817ca
   > Blocks: 0            Seconds: 5
   > contract address:    0x692AFD8EDd63cd2f82f90C380e50F685EA48c049
   > block number:        11360605
   > block timestamp:     1662883945
   > account:             0x623a6151C089CE0D8FFa5ee8640b2B8A3Ab7ed13
   > balance:             0.296204507979757376
   > gas used:            306684 (0x4adfc)
   > gas price:           1.500000008 gwei
   > value sent:          0 ETH
   > total cost:          0.000460026002453472 ETH

   Pausing for 2 confirmations...

   -------------------------------
   > confirmation number: 1 (block: 11360606)
   > confirmation number: 2 (block: 11360607)

   Deploying 'DistributorRole'
   ---------------------------
   > transaction hash:    0x240c13c5a455d3b7b272a916c16454ec93477d7ac63207b2930b66b5cfae935c
   > Blocks: 1            Seconds: 9
   > contract address:    0xF2CfEf33ce5a6B2D935Ec7d9374c07293446f576
   > block number:        11360608
   > block timestamp:     1662883990
   > account:             0x623a6151C089CE0D8FFa5ee8640b2B8A3Ab7ed13
   > balance:             0.295744499977304
   > gas used:            306672 (0x4adf0)
   > gas price:           1.500000008 gwei
   > value sent:          0 ETH
   > total cost:          0.000460008002453376 ETH

   Pausing for 2 confirmations...

   -------------------------------
   > confirmation number: 1 (block: 11360609)
   > confirmation number: 2 (block: 11360610)

   Deploying 'RetailerRole'
   ------------------------
   > transaction hash:    0x1159746b2b48628c8baa04d822f6db67b97e27cb2cb7c55b1710510a98c1888d
   > Blocks: 0            Seconds: 9
   > contract address:    0x51f3D91b78d018D134fa03894D4a655d25C50D99
   > block number:        11360611
   > block timestamp:     1662884035
   > account:             0x623a6151C089CE0D8FFa5ee8640b2B8A3Ab7ed13
   > balance:             0.295284491974850624
   > gas used:            306672 (0x4adf0)
   > gas price:           1.500000008 gwei
   > value sent:          0 ETH
   > total cost:          0.000460008002453376 ETH

   Pausing for 2 confirmations...

   -------------------------------
   > confirmation number: 1 (block: 11360612)
   > confirmation number: 2 (block: 11360613)

   Deploying 'ConsumerRole'
   ------------------------
   > transaction hash:    0x2587144f2cae470e15ef1ba1eb88343255234619bbf6f1c7b6b3cd3cafb35668
   > Blocks: 0            Seconds: 9
   > contract address:    0x772E5C0a31Ed0CE1020851659e8dD5cD790038bE
   > block number:        11360614
   > block timestamp:     1662884080
   > account:             0x623a6151C089CE0D8FFa5ee8640b2B8A3Ab7ed13
   > balance:             0.294824465972397152
   > gas used:            306684 (0x4adfc)
   > gas price:           1.500000008 gwei
   > value sent:          0 ETH
   > total cost:          0.000460026002453472 ETH

   Pausing for 2 confirmations...

   -------------------------------
   > confirmation number: 1 (block: 11360615)
   > confirmation number: 2 (block: 11360616)

   Deploying 'SupplyChain'
   -----------------------
   > transaction hash:    0x489dbc421137451a99cf3085a16296baa7bcd7e252cd17d02e03668da0ff01f1
   > Blocks: 1            Seconds: 9
   > contract address:    0x7fb78422AAd4479141112B681b378Fd31C03aC0B
   > block number:        11360617
   > block timestamp:     1662884125
   > account:             0x623a6151C089CE0D8FFa5ee8640b2B8A3Ab7ed13
   > balance:             0.291009106452048568
   > gas used:            2543573 (0x26cfd5)
   > gas price:           1.500000008 gwei
   > value sent:          0 ETH
   > total cost:          0.003815359520348584 ETH

   Pausing for 2 confirmations...

   -------------------------------
   > confirmation number: 1 (block: 11360618)
   > confirmation number: 2 (block: 11360619)
   > Saving migration to chain.
   > Saving artifacts
   -------------------------------------
   > Total cost:     0.00565542753016228 ETH

Summary
=======
> Total deployments:   6
> Final cost:          0.00599521503197448 ETH
```



## Authors

See also the list of [contributors](https://github.com/your/project/contributors.md) who participated in this project.

## Acknowledgments

* Solidity
* Ganache-cli
* Truffle
* IPFS
