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

Imagine if Microsoft Excel was better looking, had better dashboards, but for web3.

At some point, this could be turned into a plug-in for Microsoft Excel, for an easy to use UX/UI for the current large institutions.

For other insitutions, there could be a easier to use UX/UI.

---

### Open Questions

Q: Why is this necessary?
A: Web3 offers many benefits that traditional asset management, IT infrastructure, and legal systems do not via speed, efficiency, and cost. Additionally, with web3, interacting with the value chains feels more instantaneous, similar to the type of service found on regular web2 platforms if designed correctly. Additionally, the cost-saving, transparency, and compliance features are superior if designed correctly, simplifying and lowering back office costs.

Q: Do we generate the smart contract wallet first or the DAO?

A: It seems to be that the smart contract wallet is the first primitive. Based on the configuration of the wallet, specific DAO suggestions are made.

Q: What would the smart contract wallet generator look like?
A: It will probably be a factory contract that allows the creation of other wallets in a relational manner.

Q: How will complexity be managed?
A: That's tricky since many types of wallets could be created. An excellent and immediate solution would be to create roles and then define these roles with certain attributes.

Factory -> roles -> specific rules -> specific owners.

However, this can change based on the needs of institutional users. Doing user discovery with organizations could help clear up the use cases.

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
