# Stacks.js [![Test Action Badge](https://github.com/hirosystems/stacks.js/actions/workflows/tests.yml/badge.svg)](https://github.com/hirosystems/stacks.js/actions/workflows/tests.yml) [![Monorepo Version Label](https://img.shields.io/github/lerna-json/v/hirosystems/stacks.js?label=monorepo)](https://github.com/hirosystems/stacks.js/tree/main/packages)

This repo is home to most of the Stacks.js packages, which provide the building blocks to work with the [Stacks blockchain](https://www.stacks.co/what-is-stacks) from JavaScript/TypeScript.

#### Connecting Wallets

- [`@stacks/connect`](https://github.com/hirosystems/connect) Connect web application to Stacks wallet browser extensions _(separate repo)_.

#### Stacks Primitives

- [`@stacks/transactions`](https://github.com/hirosystems/stacks.js/tree/main/packages/transactions) Construct, decode transactions and work with Clarity smart contracts on the Stacks blockchain.
- [`@stacks/wallet-sdk`](https://github.com/hirosystems/stacks.js/tree/main/packages/wallet-sdk) Library for building wallets, managing accounts, and handling keys for the Stacks blockchain.
- [`@stacks/storage`](https://github.com/hirosystems/stacks.js/tree/main/packages/storage) Store and fetch files with Gaia, the decentralized storage system.
- [`@stacks/encryption`](https://github.com/hirosystems/stacks.js/tree/main/packages/encryption) Encryption functions used by stacks.js packages.
- [`@stacks/auth`](https://github.com/hirosystems/stacks.js/tree/main/packages/auth) Construct and decode authentication requests for Stacks apps.
- [`@stacks/profile`](https://github.com/hirosystems/stacks.js/tree/main/packages/profile) Functions for manipulating user profiles.
- [`@stacks/network`](https://github.com/hirosystems/stacks.js/tree/main/packages/network) Network and API library for working with Stacks blockchain nodes.
- [`@stacks/common`](https://github.com/hirosystems/stacks.js/tree/main/packages/common) Common utilities used by stacks.js packages.

#### Native Smart Contract Interaction

- [`@stacks/bns`](https://github.com/hirosystems/stacks.js/tree/main/packages/bns) Library for interacting with the BNS contract.
- [`@stacks/stacking`](https://github.com/hirosystems/stacks.js/tree/main/packages/stacking) Library for PoX stacking.

#### Others

- [`@stacks/cli`](https://github.com/hirosystems/stacks.js/tree/main/packages/cli) Command line interface to interact with auth, storage and Stacks transactions.
- `@stacks/keychain` _**DEPRECATED:** replaced by [`@stacks/wallet-sdk`](https://github.com/hirosystems/stacks.js/tree/main/packages/wallet-sdk)_

See the respective `README` in each package directory for installation instructions and usage.

---

## Documentation

Documentation and library references for the stacks.js packages are located at [stacks.js.org](https://stacks.js.org/).

### Migrating from previous versions

To migrate your app from blockstack.js to Stacks.js follow the steps in the respective [migration guide](./.github/MIGRATION.md).

## Bugs and feature requests

If you encounter a bug or have a feature request, we encourage you to follow the steps below:

 1. **Search for existing issues:** Before submitting a new issue, please search [existing and closed issues](../../issues) to check if a similar problem or feature request has already been reported.
 1. **Open a new issue:** If it hasn't been addressed, please [open a new issue](../../issues/new/choose). Choose the appropriate issue template and provide as much detail as possible, including steps to reproduce the bug or a clear description of the requested feature.
 1. **Evaluation SLA:** Our team reads and evaluates all the issues and pull requests. We are avaliable Monday to Friday and we make a best effort to respond within 7 business days.

Please **do not** use the issue tracker for personal support requests or to ask for the status of a transaction. You'll find help at the [#support Discord channel](https://discord.gg/SK3DxdsP).

## Contributing & Development

Github issues marked [help-wanted](https://github.com/hirosystems/stacks.js/labels/help-wanted)
are great places to start. Please ask in a github issue or discord before embarking
on larger issues that aren't labeled as help wanted or adding additional
functionality so that we can make sure your contribution can be included!

### Environment setup

To setup the development environment for this repository, follow these steps:

> **Prerequisites**:
> NodeJS & npm are required (v18.x.x is currently recommended)

1. Clone this package.
2. Run `npm install` to install dependencies
3. Run `npm run bootstrap` to [bootstrap](https://github.com/lerna/lerna/tree/main/commands/bootstrap) project
4. Run `npm run build` to build packages
5. Run `npm run test` to run tests

> Some tests may contain logging of errors and warnings.
> This should not be confused with failing tests.
> Make sure the last lines of `npm run test` show `lerna success - @stacks/...` for every package.

### Code of Conduct
Please read our [Code of conduct](../../../.github/blob/main/CODE_OF_CONDUCT.md) since we expect project participants to adhere to it. 

## Community

Join our community and stay connected with the latest updates and discussions:

- [Join our Discord community chat](https://discord.gg/ZQR6cyZC) to engage with other users, ask questions, and participate in discussions.

- [Visit hiro.so](https://www.hiro.so/) for updates and subcribing to the mailing list.

- Follow [Hiro on Twitter.](https://twitter.com/hirosystems)
