# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

<!-- EXAMPLE

## [1.0.0]

### Added

- I've added feature XY (#1000)

### Changed

- I've cleaned up XY (#1000)

### Deprecated

- I've deprecated XY (#1000)

### Removed

- I've removed XY (#1000)

### Fixed

- I've fixed XY (#1000)

### Security

- I've improved the security in XY (#1000)

-->

## [Unreleased]

### Added

-   `web3-rpc-methods` dependency (#5441)
-   `web3-eth-transaction-utils` dependency (#5458)
-   `getAccounts` rpc method wrapper (#5458)

### Changed

-   `Web3EthExecutionAPI` is now imported via `web3-types` instead of `web3_eth_execution_api.ts` (#5441)
-   Replace the imported methods from `rpc_methods.ts` with `ethRpcMethods` imports from `web3-rpc-methods` (#5441)
-   `Web3NetAPI` is now imported from `web3-types` instead of `web3-net` (#5441)
-   Moved `rpc_methods` tests to `web3-rpc-methods` (#5441)
-   `formatTransaction` is now imported from `web3-eth-transaction-util` instead of local import (#5458)

### Removed

-   `utils/format_transaction.ts` exports (now exported from `web3-eth-transaction-utils`) (#5458)
-   `utils/prepare_transaction_for_signing.ts` exports (now exported from `web3-eth-transaction-utils`) (#5458)
-   `detectTransactionType` export (now exported from `web3-eth-transaction-utils`) (#5458)
-   `transactionBuilder` export (now exported from `web3-eth-transaction-utils`) (#5458)
