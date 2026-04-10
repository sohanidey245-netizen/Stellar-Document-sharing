# Stellar Document Sharing dApp
<img width="1919" height="1026" alt="Screenshot 2026-04-10 125111" src="https://github.com/user-attachments/assets/de3fb75e-4f22-4f2e-882f-13a828ca7513" />

<h1>Stellar Expert Dashboard</h1>
<img width="1919" height="1026" alt="Screenshot 2026-04-10 125148" src="https://github.com/user-attachments/assets/4d568758-f0ca-405c-a4f6-5077e1a7f82e" />


## Overview

This project is a React + Vite web dApp for managing document metadata on the Stellar Soroban testnet. It provides a lightweight interface for connecting a Freighter wallet, uploading document metadata, sharing access, revoking permissions, updating document versions, and browsing stored records.

The application uses:

- `@stellar/freighter-api` for wallet connection and transaction signing
- `@stellar/stellar-sdk` for Soroban contract invocation and network access
- Vite + React for a fast development environment

## Key Features

- Connect to Freighter wallet on Stellar testnet
- Upload document metadata to a Soroban smart contract
- Share document access with another Stellar account
- Revoke previously granted access
- Update document metadata and file hash
- Fetch individual documents or list all documents
- Display document count and wallet status

## Deployed Contract

The app is configured to use the deployed testnet contract:

- Contract ID: `CCZTW4AZNPWTJEUWYD4GT6RFNAHUWNQSCKJ6ZBKZNZ2TO2PXVMUNYTY5`
- Explorer: https://stellar.expert/explorer/testnet/contract/CCZTW4AZNPWTJEUWYD4GT6RFNAHUWNQSCKJ6ZBKZNZ2TO2PXVMUNYTY5

## Project Structure

- `src/` - React application code
- `lib/stellar.js` - Stellar Soroban contract interaction layer
- `public/` - Static assets served by Vite
- `contract/` - Soroban smart contract workspace and tests

## Getting Started

### Prerequisites

- Node.js 18+ installed
- Freighter wallet extension installed
- A Stellar testnet account with test XLM

### Install Dependencies

```bash
npm install
```

### Run Locally

```bash
npm run dev
```

Open the local Vite URL shown in the terminal to use the dApp.

## How to Use

1. Open the app and connect your Freighter wallet.
2. Enter the document metadata fields.
3. Upload the document record to the Soroban contract.
4. Share with another Stellar account by entering the receiver address.
5. Use browse actions to read document records or count stored entries.

## Notes

- The current contract is deployed to Stellar testnet.
- The app is configured for the Soroban RPC endpoint: `https://soroban-testnet.stellar.org`
- `lib/stellar.js` contains the contract ID, RPC URL, and network passphrase.

## License

This project is provided as-is for demo and educational purposes.
