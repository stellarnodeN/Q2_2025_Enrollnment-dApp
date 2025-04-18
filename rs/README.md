# Rust Solana Program (`rs/`)

This sub-project contains a Solana smart contract written in Rust.

## Features
- Implements a program called `turbine_prereq` with instructions for enrollment, updating, and SOL transfers.
- Includes CLI/test functions for key generation, airdrop, transfer, and wallet conversion.

## Structure
- `src/lib.rs`: Main program logic and test functions.
- `src/programs/`: Contains the Anchor IDL-generated Rust code for the program.
- `Cargo.toml`: Rust dependencies and project metadata.
- `dev-wallet.json`, `Turbin3-wallet.json`: Example keypair files for development.

## Setup
1. Install [Rust](https://www.rust-lang.org/tools/install) and [Solana CLI](https://docs.solana.com/cli/install-solana-cli-tools).
2. Install dependencies:
   ```sh
   cd rs
   cargo build
   ```

## Usage
- Run tests (including keygen, airdrop, transfer):
  ```sh
  cargo test
  ```
- Build the program:
  ```sh
  cargo build --release
  ```
- Deploy to Solana devnet (requires Solana CLI):
  ```sh
  solana program deploy <path-to-program.so>
  ```