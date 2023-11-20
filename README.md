# Building-on-Avalanche-ETH-AVAX DegenToken Contract

This Solidity smart contract, named `DegenToken`, implements an ERC20 token with additional functionalities for managing a token shop and redemption features. The contract is developed using Solidity version ^0.8.20.

## Overview

The `DegenToken` contract inherits from OpenZeppelin's `ERC20` and `Ownable` contracts, providing basic ERC20 token functionalities along with ownership control.

## Features

### Shop Functionality

The contract includes a shop feature with predefined items and their corresponding prices:

- **Item 1:** Degen NFT (100 tokens)
- **Item 2:** Degen T-shirt & Hoodie (60 tokens)
- **Item 3:** Random IN-GAME Item (30 tokens)
- **Item 4:** Degen Sticker (10 tokens)

Users can view available shop items and their prices using the `showShopItems()` function.

### Token Management

- `mintDGN(address _to, uint256 _amount)`: Allows the contract owner to mint new Degen tokens.
- `transferDGN(address _to, uint256 _amount)`: Enables token transfer between addresses.
- `burnDGN(uint256 _amount)`: Allows users to burn (destroy) their tokens.

### Redeeming

- `redeemDGN(uint256 _item)`: Users can redeem specific items from the shop using their tokens.
- `getBalance()`: Allows users to check their token balances.

## Usage

To deploy the contract, ensure you have Solidity compiler version ^0.8.20 and the necessary dependencies from OpenZeppelin installed. Then deploy the `DegenToken` contract with the desired parameters.

Compile the contract and deploy it on a compatible Ethereum Virtual Machine (EVM) using tools like Remix, Hardhat, or Truffle.

## Authors

Andre Martee Valerio
[@Dr_EanValerio](https://twitter.com/Dr_EanValerio)


## License

This contract is licensed under the MIT License.

