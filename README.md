///Solana AirDrop Template

# Airdrop Contract for Solana

This repository contains an example airdrop contract for the Solana blockchain. The contract allows the owner to airdrop a specified number of tokens to a list of recipient addresses.

## Prerequisites

- Rust compiler and tools: Follow the instructions at [https://www.rust-lang.org/tools/install](https://www.rust-lang.org/tools/install) to install the Rust compiler and tools.

- Solana CLI: Follow the instructions at [https://docs.solana.com/install/](https://docs.solana.com/install/) to install the `solana` command-line interface (CLI).

## Compiling the Contract

To compile the contract, run the following command in the root directory of the repository:

cargo build --release


This will build the contract and generate a file called `target/release/airdrop_contract.so`.

## Deploying the Contract

To deploy the contract to the Solana network, you will need to have a Solana account with some SOL tokens in it to pay for the transaction fees.

Use the `solana` CLI to sign and submit a transaction to create a new instance of the contract on the blockchain. For example:

CLI to sign and submit a transaction to execute the airdrop. For example:

solana transfer <owner_sk> <airdrop_contract_pubkey> <receiver_pubkey> <amount>

Copy code

Replace `<owner_sk>` with the private key of the contract owner, `<airdrop_contract_pubkey>` with the public key of the contract account, `<receiver_pubkey>` with the public key of the recipient account, and `<amount>` with the number of tokens to be airdropped.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

This contract was developed using the [Solana SDK](https://github.com/solana-labs/solana-sdk) and the [Solana Rust Starter Kit](https://github.com/solana-labs/solana-rust-starter-kit). chatGPT (openai) for this wonderful README.
