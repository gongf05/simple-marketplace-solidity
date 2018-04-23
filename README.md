# Prototype Implementation of Data MarketPlace 

```
name: Implement a prototype data marketplace 
type: development
status: initial draft
editor: Fang Gong <fang@oceanprotocol.com>
date: 04/16/2018 (updated: 04/18/2018)
```

## Objective

This PoC implements a prototype publishing/consuming marketplace using Solidity. It resolves the issue in [https://github.com/oceanprotocol/research/issues/11](https://github.com/oceanprotocol/research/issues/11)

Requirements:

* Working code published in a GitHub repository
* Project should include unit tests
* Project should be deployed in Ropsten network
* Project should include documentation to understand the software architecture, 
* testing and deployment procedure
* Project can use Truffle & OpenZeppeling frameworks

## Features:
* Version 1.0 (04/17/2018): 
	* `struct Asset`: it stores the information of data asset including name, provider, price and balance.
	* `ERC20 token`: it supports ERC20 token in the marketplace which can be customized with parameters.
	* `publish` function: user can register new data asset using `publish` function.
	* `purchase` function: user can purchase the data asset by making payment of ERC20 token.
	* `withdraw` function: owner can withdraw the balance of data asset to his own wallet.
	* `unit testing`: the unit testing can validate the correctness of each function using truffle framework.
	* `OpenZeppelin`: it uses the OpenZeppelin framework to prevent potential error in smart contracts.
	* frontend: user can interact with the smart contracts using MetaMask.

## Implementation and Documentation

We had implemented the smart contracts, unit tests, and front end using testRPC and Ropsten testnet. Please refer to specific document for details.

Folder Name  |  Content Description | README / DEMO 
--- | --- | --- |
code_testrpc | prototype with TestRPC | [readme](code_testrpc/README.md)
code_ropsten | prototype with Ropsten | [readme](code_ropsten/README.md)

## Future Work:

* modify testing file for Ropsten testing;
* add more functionality in smart contracts;
* add more testing for better coverage.
