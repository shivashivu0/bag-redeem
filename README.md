# Token Contract 

This README provides an overview of the Token contract and its functionalities.

## Overview

The Token contract is a Solidity smart contract developed on the Ethereum blockchain. It serves as a basic example of a token contract that allows minting, burning, transferring tokens, as well as redeeming and purchasing bags using these tokens.

## Contract Functionality

### ERC20 Token Features

The contract inherits from the ERC20 standard, providing basic token functionalities such as:

- Minting tokens: `mintTokens(address account, uint256 amount)`
- Burning tokens: `burnTokens(uint256 amount)`
- Transferring tokens: `transferTokens(address recipient, uint256 amount)`

### Bag Redemption and Purchase

The contract also includes functionality for redeeming and purchasing bags using tokens. Each bag has a specific cost and a limited quantity available for redemption or purchase. The bags available for redemption or purchase are:

- Backpack
- Sling Bag
- Tote
- Messenger Bag

The bag redemption and purchase functions are:

- `redeemBag(string memory bag, uint256 sum)`: Allows users to redeem a specified quantity of a bag by providing the bag type and the quantity.
- `purchaseBag(string memory bag)`: Allows users to purchase a single bag of a specified type.

### Events

The contract emits the following events:

- `LogMessage(string message)`: Indicates various informational messages.
- `BagsRedeemed(address indexed account, string bag, uint256 quantity)`: Indicates when bags are redeemed, specifying the user, bag type, and quantity.

## Usage

To interact with the contract, users can call the provided functions using Ethereum wallets or through smart contract interactions.

## Development

The contract is developed using Solidity version 0.8.0 and utilizes OpenZeppelin contracts for ERC20 token functionality and access control through Ownable. It's recommended to review the code and ensure its compatibility and security for your specific use case before deployment.

## License

This project is licensed under the MIT License. You can find the license information in the SPDX-License-Identifier tag within the contract file.

## Author

Shivakumar 

shivashivu2499@gmail.com
