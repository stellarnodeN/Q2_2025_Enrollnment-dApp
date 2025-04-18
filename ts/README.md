# TypeScript Solana Client (`ts/`)

This sub-project provides TypeScript scripts and utilities to interact with Solana and the on-chain program.

## Features
- Scripts for airdrop, SOL transfer, key generation, wallet conversion, and program enrollment.
- Uses `@solana/web3.js` and `@coral-xyz/anchor` for Solana and Anchor program interaction.

## Structure
- `airdrop.ts`, `transfer.ts`, `transfer-all.ts`: Scripts for SOL operations.
- `keygen.ts`, `key-converter.ts`: Wallet utilities.
- `enroll.ts`: Script to enroll with the on-chain program.
- `programs/`: Anchor IDL and program types.
- `package.json`, `tsconfig.json`: Project configuration and dependencies.

## Setup
1. Install [Node.js](https://nodejs.org/) and [Yarn](https://yarnpkg.com/) or npm.
2. Install dependencies:
   ```sh
   cd ts
   yarn install
   # or
   npm install
   ```

## Usage
- Run a script (example: airdrop):
  ```sh
  yarn airdrop
  # or
  npx ts-node airdrop.ts
  ```
- See `package.json` scripts for more commands:
  - `keygen`, `key-converter`, `airdrop`, `transfer`, `transfer-all`, `enroll`

## Notes
- Update wallet files as needed for your own development.
- Scripts use devnet by default.