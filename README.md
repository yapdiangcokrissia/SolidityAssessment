# MyToken

A simple token contract made in Solidity is called MyToken. It symbolizes a simple token with minting and burning functionality. This project's goal is to offer a model for making unique tokens on the Ethereum blockchain.

## Features

- **Token Name**: The token has a public variable `tokenName` which represents the name of the token. It is initialized with the value "SEVENTEEN".

- **Token Abbreviation**: The token also has a public variable `tokenAbbrv` which represents the abbreviation of the token. It is initialized with the value "SVT".

- **Total Supply**: The token keeps track of the total supply using the public variable `totalSupply`. It is initialized with the value 0.

- **Balances**: The token uses a mapping variable `balances` to associate each address with a uint value representing the balance of that address. The `balances` mapping is publicly accessible.

- **Mint Function**: The contract includes a `mint` function which can be called to increase the total supply and add tokens to a specific address. This function takes two parameters: `_address` (the address to receive the tokens) and `_value` (the amount of tokens to be minted).

- **Burn Function**: The contract also includes a `burn` function which can be called to decrease the total supply and remove tokens from a specific address. This function takes two parameters: `_address` (the address from which tokens will be burned) and `_value` (the amount of tokens to be burned). It checks if the balance of the `_address` is greater than or equal to the `_value` before performing the burn operation.

## Usage

To use the MyToken contract, you can deploy it on the Ethereum blockchain using a development environment like Remix. Once deployed, you can interact with the contract by calling the `mint` and `burn` functions to manage the token supply and balances.

Note that this is a simple token contract and that it should only be used for learning or as a starting point for complex token contracts. It does not provide options for managing ownership or moving tokens between addresses.

## License

This project is licensed under the [MIT License](LICENSE). Feel free to use and modify the code according to your needs.
