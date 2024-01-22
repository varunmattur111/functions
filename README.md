## Token Smart Contract 

## Overview
This Solidity smart contract is an implementation of a standard ERC-20 token with additional functionality to mint, burn, and transfer tokens. The contract extends the OpenZeppelin ERC20 contract to leverage well-tested and secure token functionality.

## Features
ERC-20 Compliance: The Token contract adheres to the ERC-20 standard, providing basic token functionalities like transfer, balance inquiry, and approval mechanisms.

## Constructor Initialization:
 The contract's constructor initializes the token with a specified title, code, decimals, and magnitude, minting an initial supply to the deployer's address.

## Minting Tokens:
 The contract includes a mintTokens function, allowing the contract deployer to mint additional tokens. Only the deployer (contracter) has the authority to mint new tokens.

## Burning Tokens:
 The contract provides a burnTokens function to allow users to burn their own tokens, reducing the total token supply.

## Transfer Tokens:
 The contract includes a custom transferTokens function that wraps the standard transfer function from the ERC-20 standard, providing a simplified interface for token transfers.

## Usage
Deployment:

Deploy the contract to the Ethereum blockchain, specifying the necessary parameters (token title, code, decimals, and magnitude).
The deployer becomes the initial holder of the entire token supply.
Minting Tokens:

Call the mintTokens function to mint additional tokens. Only the deployer can execute this function.
Burning Tokens:

Call the burnTokens function to burn a specified amount of tokens from the sender's balance.
Transferring Tokens:

Use the transferTokens function to transfer tokens to another address. This function wraps the standard ERC-20 transfer function.

## Requirements
Solidity Compiler v0.8.0 
OpenZeppelin Contracts Library

## Author

Varun
