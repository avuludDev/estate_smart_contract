# # Truestate Contract

The Truestate contract is a Solidity smart contract that allows for the creation and management of individual ERC20 token contracts, each representing a separate "project" or "object". These projects can be used for a variety of purposes, such as crowdfunding, fundraising, or asset tokenization.

The contract provides a number of functions for creating and managing these individual projects, including the ability to create new projects, view project balances, burn tokens, and set minimum deposit amounts. The contract also uses two price aggregator contracts to determine the current exchange rate for Ether and other currencies.

## Getting Started

To get started with the Truestate contract, you'll need to have a working Ethereum development environment set up, such as Truffle or Remix. Once you have your environment set up, you can deploy the Truestate contract to your local blockchain or test network.

## Usage

Once the Truestate contract is deployed, you can use the following functions to create and manage individual projects:

### `createProject(uint256 _supply)`

Creates a new project with the specified token supply.

### `getContractAddressByID(uint256 _id)`

Returns the address of the token contract for the specified project ID.

### `getBalanceByID(uint256 _id)`

Returns the current token balance for the specified project ID.

### `burn(uint256 _id)`

Burns all tokens for the specified project ID.

### `setMinAmountByID(uint256 _minAmount, uint256 _id)`

Sets the minimum deposit amount for the specified project ID.

### `getMinAmountByID(uint256 _id)`

Returns the minimum deposit amount for the specified project ID.

### `getAdmin()`

Returns the address of the payment wallet.

### `setAdmin(address account)`

Sets the address of the payment wallet.

### `getRate()`

Returns the current exchange rate for Ether and other currencies.

## Contributing

Contributions to the Truestate contract are welcome and encouraged! To contribute, simply fork the repository, make your changes, and submit a pull request.

## License

The Truestate contract is released under the [MIT License](https://opensource.org/licenses/MIT).
