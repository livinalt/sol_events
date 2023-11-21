# ICO Platform Smart Contract

## Overview

The ICO Platform Smart Contract is a Solidity contract designed for an Initial Coin Offering (ICO) platform. It enables users to purchase tokens, transfer tokens between addresses, check the token circulation, and determine if the ICO has expired.

## Contract Details

- **Token Name:** Miva
- **Token Abbreviation:** MVA
- **Initial Token Supply:** 1000

## Events

1. Token Purchased
   - Triggered when a user successfully purchases tokens during the ICO.
   - Event: `Purchased(address indexed _address, uint amount)`

2. Token Transfer
   - Triggered when tokens are transferred between two addresses.
   - Event: `Transfer(address indexed _addressOne, address indexed _addressTwo, uint amount)`

## Functions

1. Token Purchase
   - Function: `purchased(address _address, uint256 amount) public payable`
   - Description: Allows users to purchase tokens during the ICO.

2. Token Transfer
   - Function: `transfer(address addressOne, address addressTwo, uint _amount) public payable`
   - Description: Facilitates the transfer of tokens between two addresses.

3. Check Token Circulation
   - Function: `circulation(uint256 amount) public payable returns(uint256)`
   - Description: Shows the balance of token supply after a specified circulation.

4. Check ICO Expiry
   - Function: `expire() public payable returns(string memory)`
   - Description: Indicates whether the ICO has expired based on the token supply.

## Usage

1. Deployment
   - Deploy the contract to your chosen Ethereum network.

2. Token Purchase
   - Use the `purchased` function to participate in the ICO and buy tokens.

3. Token Transfer
   - Utilize the `transfer` function to transfer tokens between addresses.

4. Check Token Circulation
   - Call the `circulation` function to view the remaining token supply.

5. Check ICO Status
   - Use the `expire` function to check if the ICO has expired.
  
## License

This project is licensed under the MIT License.

- [Solidity Compiler](https://docs.soliditylang.org/en/latest/installing-solidity.html)
- [Ethereum Development Environment](https://ethereum.org/en/developers/docs/development-environment/)

