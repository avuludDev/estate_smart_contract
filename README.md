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


# TruEstateObject

`TruEstateObject` is an ERC20-compatible token smart contract implemented on Ethereum. The token contract is deployed on the Ethereum Mainnet and it's used to represent ownership of an asset in the real estate sector.

## Functionalities

The `TruEstateObject` token contract provides the following functionalities:

-   `totalSupply()`: returns the total number of tokens in circulation.
-   `balanceOf(address account)`: returns the token balance of the specified account.
-   `transfer(address recipient, uint256 amount)`: transfers a specified amount of tokens to the recipient address.
-   `allowance(address owner, address spender)`: returns the remaining number of tokens that spender will be allowed to spend on behalf of owner through `transferFrom`.
-   `approve(address spender, uint256 amount)`: sets the `amount` of tokens that `spender` is allowed to transfer on behalf of the `msg.sender`.
-   `transferFrom(address sender, address recipient, uint256 amount)`: moves the `amount` of tokens from `sender` to `recipient` using the allowance mechanism.
-   `increaseAllowance(address spender, uint256 addedValue)`: increases the `spender` allowance by `addedValue`.
-   `decreaseAllowance(address spender, uint256 subtractedValue)`: decreases the `spender` allowance by `subtractedValue`.
-   `name()`: returns the name of the token.
-   `symbol()`: returns the symbol of the token.
-   `decimals()`: returns the number of decimal places used for the token.
-   `minbuy()`: returns the minimum amount of tokens required to purchase.
-   `initialize(string memory name_, string memory symbol_, uint256 initialSupply)`: initializes the token contract with the given `name_`, `symbol_` and `initialSupply`.

## Variables

The `TruEstateObject` token contract has the following variables:

-   `_balances`: a mapping of user addresses to their token balances.
-   `_allowances`: a mapping of user addresses to a mapping of addresses allowed to spend tokens on behalf of that user.
-   `_totalSupply`: the total number of tokens in circulation.
-   `payoutDone`: a boolean that determines whether or not dividends have been paid out.
-   `payoutDate`: the date at which dividends will be paid out.
-   `_dividends`: the value of the dividends to be paid out.
-   `_minbuy`: the minimum amount of tokens required to purchase.
-   `holdersCount`: the number of token holders.
-   `holders`: a mapping of token holders' indexes to their addresses.
-   `expireTerm`: the amount of time (in seconds) before dividends expire.
-   `_decimals`: the number of decimal places used for the token.
-   `_name`: the name of the token.
-   `_symbol`: the symbol of the token.

## Events

The `TruEstateObject` token contract emits the following event:

-   `DividendClaim(address indexed _account, address indexed _contract, uint256 _tokens, uint256 _ethereum)`: emitted when a token holder claims dividends.

## Deployment

The `TruEstateObject` token contract has been deployed on the Ethereum Mainnet.

## Authors

-   [@avuludDev](https://github.com/avuludDev)
- 
