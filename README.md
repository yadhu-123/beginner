# MyToken Contract

This is a simple Solidity smart contract for creating a custom ERC-20 token called "META" (MTA).

## Contract Details

- *Token Name*: META
- *Token Abbreviation*: MTA
- *Total Supply*: 0 (initially)

## Public Variables

- `tokenName`: A public string variable representing the name of the token.
- `tokenAbbrv`: A public string variable representing the abbreviation of the token (symbol).
- `totalSupply`: A public unsigned integer variable representing the total supply of the token.

## Mapping Variable

- `balances`: A mapping that associates addresses with their corresponding token balances. It tracks the number of tokens held by each address.

## Functions

### `mint`

solidity
function mint(address _address, uint _value) public


This function allows the contract owner (or anyone with the appropriate permissions) to mint new tokens and assign them to a specific address.

- Parameters:
  - `_address`: The address to which the newly minted tokens will be assigned.
  - `_value`: The number of tokens to mint and assign.

### `burn`

solidity
function burn(address _address, uint _value) public


The `burn` function allows the contract owner (or anyone with the appropriate permissions) to burn a specific number of tokens held by a given address.

- Parameters:
  - `_address`: The address from which tokens will be burned.
  - `_value`: The number of tokens to burn.

Please note that burning tokens reduces the total supply of the token, and it can only be executed if the balance of the target address is equal to or greater than the number of tokens to be burned.

## License

This smart contract is licensed under the MIT License.

plaintext
SPDX-License-Identifier: MIT


## Disclaimer

This smart contract is provided as-is and without any warranties. Use it at your own risk.

*Note*: Remember to mention the Solidity version used to compile the contract in your actual README file. Since Solidity is constantly evolving, it is important to specify the version to ensure future developers can compile and understand the code correctly.
