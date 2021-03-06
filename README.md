# signature-registry

[![Build Status][travis-image]][travis-url]
[![Solidity Coverage Status][coveralls-image]][coveralls-url]

[travis-image]: https://travis-ci.org/parity-contracts/signature-registry.svg?branch=master
[travis-url]: https://travis-ci.org/parity-contracts/signature-registry
[coveralls-image]: https://coveralls.io/repos/github/parity-contracts/signature-registry/badge.svg?branch=master
[coveralls-url]: https://coveralls.io/github/parity-contracts/signature-registry?branch=master

Decentralized registry of 4-bytes signatures to method mappings

## Deployments

- Mainnet: [`0x44691B39d1a75dC4E0A0346CBB15E310e6ED1E86`](https://etherscan.io/address/0x44691B39d1a75dC4E0A0346CBB15E310e6ED1E86)

## Getting started

This project uses the [Truffle](http://truffleframework.com/) framework. To install the required
dependencies run:

```
yarn install
```

To run the test suite:

```
yarn test
```

## Usage

A truffle script can be used to register many function signatures to the mainnet registry:
```
npx truffle exec --network mainnet scripts/register-many.js "a()" "b(uint256)" ...
```