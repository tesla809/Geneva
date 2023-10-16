## Project: Geneva

### Design Statement

How might we improve the creation and management of smart contract wallets, so that institutions can manage the assets securely, scaleable, and more efficiently?

## Goal

The goal is to create a smart contract wallet generator that has features that:

- appeals to institutions to help reduce the complexities of managing assets.
- is composable to allow developers to integrate and expand upon it: Think Salesforce for web3.
- is open-ended enough to allow for up sales on treasury management and banking services that simplify back office operations and compliance.
- allows for easy setup and management by nontechnical people.
- allows for easy integration of KYC (know your customer), KYT (know your transaction), and AML (Anti-money laundering).
- is general purpose enough to create any organization.

Using composable wallets as a primitive, one can build emergent and complex organizations that feel lightweight and manageable while leveraging the interoperability, speed, and convenience of web3. This opens the door for lower cost structures, greater security, better asset management, and a more user-friendly and streamlined experience for institutional and end users.

For the old heads, it's Lotus123, but for web3.

---

## Foundry Set Up

**Foundry is a blazing fast, portable and modular toolkit for Ethereum application development written in Rust.**

Foundry consists of:

- **Forge**: Ethereum testing framework (like Truffle, Hardhat and DappTools).
- **Cast**: Swiss army knife for interacting with EVM smart contracts, sending transactions and getting chain data.
- **Anvil**: Local Ethereum node, akin to Ganache, Hardhat Network.
- **Chisel**: Fast, utilitarian, and verbose solidity REPL.

## Documentation

https://book.getfoundry.sh/

## Usage

### Build

```shell
$ forge build
```

### Test

```shell
$ forge test
```

### Format

```shell
$ forge fmt
```

### Gas Snapshots

```shell
$ forge snapshot
```

### Anvil

```shell
$ anvil
```

### Deploy

```shell
$ forge script script/Counter.s.sol:CounterScript --rpc-url <your_rpc_url> --private-key <your_private_key>
```

### Cast

```shell
$ cast <subcommand>
```

### Help

```shell
$ forge --help
$ anvil --help
$ cast --help
```
