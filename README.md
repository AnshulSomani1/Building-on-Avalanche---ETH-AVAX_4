# Building-on-Avalanche---ETH-AVAX_4

# Token Smart Contract

This Solidity smart contract implements a basic ERC20-like token with minting, burning, transfer, and redeem functions.

## Contract Details

- **Token Name:** TOKEN
- **Token Symbol:** TKN
- **Decimals:** 18

## Features

1. **Mint Tokens**
   - Only the contract owner can mint new tokens.
   - Increases the total supply and the balance of the specified recipient.

2. **Burn Tokens**
   - Allows burning of tokens from a specified address.
   - Decreases the total supply and the balance of the specified address.

3. **Transfer Tokens**
   - Enables transfer of tokens between addresses.
   - Requires the sender to have a sufficient balance.

4. **Redeem Tokens**
   - Allows redeeming tokens for in-game items.
   - Requires different minimum amounts based on the item type.

## Functions

- `mint(address to, uint256 value)`
  - Mints `value` tokens to the address `to`.

- `burn(address account, uint256 value)`
  - Burns `value` tokens from the address `account`.

- `transfer(address recipient, uint256 value)`
  - Transfers `value` tokens from the sender to the address `recipient`.

- `redeem(address beneficiary, uint256 value, uint256 item)`
  - Redeems `value` tokens from `beneficiary` for a specific `item`.

## Redeemable Items

- **Item 1:** Requires 50 tokens.
- **Item 2:** Requires 100 tokens.
- **Item 3:** Requires 200 tokens.

## Usage

1. **Deploy the Contract**
   - Deploy the contract to a compatible Ethereum network.

2. **Mint Tokens**
   - Use `mint()` to create new tokens and assign them to an address.

3. **Transfer Tokens**
   - Use `transfer()` to send tokens from one address to another.

4. **Burn Tokens**
   - Use `burn()` to remove tokens from circulation.

5. **Redeem Tokens**
   - Use `redeem()` to exchange tokens for game items.

## License

This project is licensed under the MIT License.
