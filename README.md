# Token Smart Contract 

## Overview

This is a simple Ethereum smart contract written in Solidity that implements a basic ERC-20 token with additional functionalities. The contract is named "Token" and includes features such as minting, burning, transferring tokens, redeeming game items, checking balances, and sharing game items.

## Smart Contract Details

### ERC-20 Token Standard

The smart contract adheres to the ERC-20 token standard, providing basic token functionalities like transferring, minting, and burning.

### Additional Features

1. **Minting:**
   - Only the owner of the contract can mint new tokens.
   - The `mint` function allows the owner to mint a specified quota of tokens and assign them to a designated legatee.

2. **Burning:**
   - The owner can burn a specified quota of tokens using the `burn` function.

3. **Transferring Tokens:**
   - Users can transfer a specified quota of tokens to another address using the `transferTokens` function.

4. **Redeeming Game Items:**
   - Users can redeem in-game items such as Sword, Shield, and Pistol by burning a specific quota of tokens. The redemption details are specified in the `redeemGameItem` function.

5. **Checking Balances:**
   - Users can check the token balance of a designated legatee using the `checkBalance` function.

6. **Sharing Game Items:**
   - Users can share game items with a designated legatee by emitting a `RewardShared` event. This function is triggered using the `shareGameItem` function.

## Usage

1. **Deployment:**
   - Deploy the smart contract to the Ethereum blockchain, specifying the initial token supply and the address of the initial legatee.

2. **Minting:**
   - The owner can mint additional tokens using the `mint` function, assigning the new tokens to a specific legatee.

3. **Burning:**
   - The owner can burn tokens from their own balance using the `burn` function.

4. **Transferring Tokens:**
   - Users can transfer tokens to another address using the `transferTokens` function.

5. **Redeeming Game Items:**
   - Users can redeem in-game items by calling the `redeemGameItem` function and specifying the desired game item.

6. **Checking Balances:**
   - Users can check the token balance of a designated legatee using the `checkBalance` function.

7. **Sharing Game Items:**
   - Users can share game items with a designated legatee using the `shareGameItem` function.

## Events

The smart contract emits several events to track important actions:

- `PlayerRewarded`: Triggered when a player (legatee) is rewarded with a specific quota of tokens.
- `ItemRedeemed`: Triggered when a player redeems a game item, specifying the item name and the cost in tokens.
- `PlayerBalanceChecked`: Triggered when a player checks their token balance.
- `RewardShared`: Triggered when a user shares a game item with a legatee.

## Author 

aravind.p866@gmail.com
