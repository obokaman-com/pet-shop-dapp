# Pet Shop example dApp

This repository contains the needed code (Solidity smart contracts, and other assets) to run a pet shop example dApp running on a Ethereum Virtual Machine (EVM) compatible blockchain running in local, using [Ganache](https://trufflesuite.com/ganache/), and other tools from the [Truffle Suite](https://trufflesuite.com/).

## Introduction

This codebase is the result of following the full tutorial available at [https://trufflesuite.com/tutorial/](https://trufflesuite.com/tutorial/). I highly encourage you to follow the full tutorial to fully understand what is happening behind the scenes.

## Requirements

You will need to install the following software to run this code:
- [Git](https://git-scm.com/)
- [Node.js v8+ LTS & npm](https://nodejs.org/en/)
- [Ganache](https://trufflesuite.com/ganache/)

## Running

After installing the needed software, execute the following commands to have the full example running:

#### 1. Installing needed node libraries and dependencies.
```shell
$ npm install
```

#### 2. Starting a local EVM blockchain using Ganache

Simply execute the Ganache executable file you've previously downloaded & installed

#### 3. Link your local project into Ganache

Go to Contracts tab and link the `truffle-config.js` file you'll find in your local project. This will help Ganache to add some interesting data to your transactions when we interact with the smart contracts.

#### 4. Compiling and deploying your smart contracts to the local blockchain
```shell
$ truffle compile && truffle migrate
```

#### 5. Run a local web server to visualize your dApp
```shell
$ npm run dev
```

#### 6. Configure your Metamask 

You should add an additional network using your Ganache RPC server, and should also add an additional wallet. You can use the private key from the first available virtual wallet. (More information, screenshots and instructions on the tutorial page.)

#### 7. Play!

When you go to `http://localhost:3000/` you will find your Pet Shop. If you followed the previous steps, Metamask should ask you for permission to connect to your local wallet, and you should be able to adopt dogs. Every time you adopt a dog, Metamask will ask for permission for the transaction, and gas will be deducted from your virtual wallet.

Enjoy!

---

Full credits to **Truffle Suite** and its tutorial guide at [https://trufflesuite.com/tutorial/](https://trufflesuite.com/tutorial/)
