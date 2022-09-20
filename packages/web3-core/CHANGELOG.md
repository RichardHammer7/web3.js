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

### Changed

-   `privateKey` argument for `TransactionBuilder` type was changed from `HexString | Buffer` to `{ privateKey: HexString | Buffer; privateKeyToAddress: privateKeyToAddress }` (#5458)
-   Return type for `TransactionBuilder` type was changed from `Promise<ReturnType>` (with `ReturnType` being a generic) to `Promise<Transaction>` (`Transaction` from `web3-types`) (#5458)
