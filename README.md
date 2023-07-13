# MyToken

MyToken is a basic token contract implemented in Solidity. It represents a simple token with minting and burning functionality. The purpose of this project is to provide a template for creating custom tokens on the Ethereum blockchain.

## Features

- **Token Name**: The token has a public variable `tokenName` which represents the name of the token. It is initialized with the value "SEVENTEEN".

- **Token Abbreviation**: The token also has a public variable `tokenAbbrv` which represents the abbreviation of the token. It is initialized with the value "SVT".

- **Total Supply**: The token keeps track of the total supply using the public variable `totalSupply`. It is initialized with the value 0.

- **Balances**: The token uses a mapping variable `balances` to associate each address with a uint value representing the balance of that address. The `balances` mapping is publicly accessible.

- **Minting**: The contract includes a `mint` function which can be called to increase the total supply and add tokens to a specific address. This function takes two parameters: `_address` (the address to receive the tokens) and `_value` (the amount of tokens to be minted).

- **Burning**: The contract also includes a `burn` function which can be called to decrease the total supply and remove tokens from a specific address. This function takes two parameters: `_address` (the address from which tokens will be burned) and `_value` (the amount of tokens to be burned). It checks if the balance of the `_address` is greater than or equal to the `_value` before performing the burn operation.

## Usage

To use the MyToken contract, you can deploy it on the Ethereum blockchain using a development environment like Remix or Truffle. Once deployed, you can interact with the contract by calling the `mint` and `burn` functions to manage the token supply and balances.

Please note that this is a basic token contract and should be used for educational purposes or as a starting point for more complex token contracts. It does not include features like transferring tokens between addresses or managing ownership.

## License

This project is licensed under the [MIT License](LICENSE). Feel free to use and modify the code according to your needs.
