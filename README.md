# ETH3

## AUTHOR

John Bulos https://github.com/Leno901

# MyToken ERC-20 Contract

MyToken is an Ethereum ERC-20 token contract written in Solidity. It extends the functionality of the OpenZeppelin ERC-20 contract and includes ownership features from the Ownable contract.

## Overview

This contract allows for the creation of a customizable ERC-20 token with the ability to mint new tokens, burn existing tokens, and manage ownership.

## Features

- Minting: The contract owner can mint new tokens and assign them to a specified address.
- Burning: Any user can burn their own tokens.
- Transfer: Allows users to transfer tokens from one address to another.

## Prerequisites

- [Solidity Compiler](https://docs.soliditylang.org/en/v0.8.0/installing-solidity.html)
- [OpenZeppelin Contracts](https://github.com/OpenZeppelin/openzeppelin-contracts)

## Steps
Compile Contract:
Compile the contract using the Solidity compiler. You can use tools like Remix or Hardhat for this purpose.

Deploy Contract:
Deploy the compiled contract to an Ethereum network, providing the necessary parameters for the constructor.

## USAGE

- Mint Tokens:
Use the mint function to mint new tokens and assign them to a specified address.

- Burn Tokens:
Use the burn function to burn a specified amount of tokens owned by the sender.

- Transfer Tokens:
Use the standard transfer and transferFrom functions to transfer tokens between addresses.

## EXAMPLE

// Deploy MyToken contract with initial supply of 1 million tokens
MyToken myToken = new MyToken("MyToken", "MTK", 1000000, msg.sender);

// Mint 500,000 tokens and assign them to another address
myToken.mint(address2, 500000);

// Burn 100,000 tokens from the sender's address
myToken.burn(100000);

// Transfer 200,000 tokens from sender to another address
myToken.transfer(address3, 200000);

or

See video demonstration:
```bash
https://www.loom.com/share/3844b6f9b3a34d738da2459782c0354f?sid=5a1fe1e7-4448-4ff6-9215-8f2f7588e748

