# MyToken 

## Overview

MyToken is a simple ERC-20 compliant token smart contract built on the Ethereum blockchain. The contract includes basic functionalities such as token minting, burning, and transfer. It is based on the OpenZeppelin library, utilizing the ERC20 and Ownable contracts.

## Contract Details

### Token Information

- **Name**: Token
- **Symbol**: Tk
- **Decimals**: 0

The initial token supply is set to 50 and is assigned to the deployer of the contract.

### Contract Inheritance

MyToken inherits from two main contracts:

1. **ERC20**: This is an implementation of the ERC-20 standard, providing basic functionality such as transferring tokens, checking balances, and approving spending.

2. **Ownable**: This contract ensures that only the owner (deployer) has certain privileges, such as the ability to mint new tokens.

## Contract Functions

### Mint Tokens

The owner of the contract can mint additional tokens and assign them to a specified address.

```solidity
function mintTokens(address recipient, uint256 amount) public onlyOwner
```

### Burn Tokens

Token holders can burn a certain amount of their tokens, reducing the total supply.

```solidity
function burnTokens(uint256 amount) public
```

### Transfer Tokens

Token holders can transfer tokens to another address.

```solidity
function transferTokens(address to, uint256 amount) public returns (bool)
```

### Get Total Token Supply

Retrieve the total supply of the token.

```solidity
function getTotalSupply() public view returns (uint256)
```

### Get Token Decimals

Retrieve the number of decimals used by the token.

```solidity
function getTokenDecimals() public view returns (uint8)
```

## License

This smart contract is released under the MIT License. See the SPDX-License-Identifier tag in the source code for details.

## Usage

1. Deploy the smart contract to the Ethereum blockchain.
2. Interact with the contract using functions like `mintTokens`, `burnTokens`, and `transferTokens`.
3. Only the owner has permission to mint new tokens.


**Author**: [Nikhil Chandha]

