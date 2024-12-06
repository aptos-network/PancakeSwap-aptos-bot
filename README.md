# Aptos Sniper Bot with PancakeSwap Integration

This Python-based sniper bot interacts with the Aptos blockchain network and supports token swaps on decentralized exchanges (DEXs) like PancakeSwap. The bot performs the following key actions:

1. **Transaction Signing**: The bot can simulate signing Aptos transactions using the user's private key.
2. **Aptos Transaction Sending**: It sends the signed transactions to the Aptos network to transfer assets between wallets.
3. **Wallet Balance Checking**: It checks the current balance of an Aptos wallet using the Aptos API.
4. **Token Swapping**: The bot allows users to swap tokens on DEXs, such as PancakeSwap, by interacting with their respective APIs.

## Features:

- **Aptos Network Integration**: Communicates with the Aptos blockchain for transaction management.
- **Token Swap Capability**: Supports token swaps between different tokens on a DEX (like PancakeSwap).
- **Private Key Handling**: Handles transaction signing with a private key (Ed25519 format).
- **Error Handling**: Robust error handling mechanisms for network issues and transaction failures.

## Configuration:

- **APTOS_API_URL**: The API URL for interacting with the Aptos blockchain.
- **PRIVATE_KEY**: The user's private key (used to sign transactions).
- **WALLET_ADDRESS**: The user's Aptos wallet address.
- **RECIPIENT_ADDRESS**: The recipient's wallet address (for sending transactions).
- **AMOUNT**: The amount to send in the smallest unit of the token.

## How It Works:

1. **Check Balance**: The bot starts by checking the balance of the provided Aptos wallet address.
2. **Swap Tokens**: It then performs a token swap operation on a DEX (PancakeSwap, for example).
3. **Send Transaction**: Finally, the bot signs and sends the transaction to the Aptos network to transfer assets to a recipient address.

## Dependencies:

- `requests` for making HTTP requests.
- `eth_account` for signing transactions.
- `json` for handling JSON responses.

## Usage:

To use this bot, you need to set your Aptos private key and wallet address as environment variables (`APTOS_PRIVATE_KEY` and `APTOS_WALLET_ADDRESS`). Replace the recipient address and token swap parameters as needed.
