# StarToken Smart Contract

The `StarToken` smart contract is an Ethereum-based token implementation that allows minting and burning of tokens. The contract includes basic functionalities for handling token supply and balances, ensuring a straightforward and secure way to manage tokens.

## Features

1. **Token Details**: Public variables store the token name, abbreviation, and total supply.
2. **Balances Mapping**: A mapping from addresses to their respective balances.
3. **Mint Function**: Increases the total supply and the balance of a specified address.
4. **Burn Function**: Decreases the total supply and the balance of a specified address with necessary checks to prevent burning more tokens than available.

## Contract Details

### Public Variables

- `tokenName`: The name of the token, set to "StarToken".
- `tokenAbbrv`: The abbreviation of the token, set to "STR".
- `totalSupply`: The total supply of the token, initially set to 0.

### Mappings

- `balances`: Maps addresses to their token balances.

### Functions

#### `mint`

This function allows the creation of new tokens. It increases the total supply and the balance of the specified address.

**Parameters:**
- `_to`: The address to which the tokens will be minted.
- `_value`: The number of tokens to mint.

**Usage:**
```solidity
function mint(address _to, uint256 _value) public {
    totalSupply += _value;
    balances[_to] += _value;
}
