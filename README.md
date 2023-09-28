# Cosmos Address Labeling Repository

This repository contains a dataset of Cosmos addresses and their associated labels and tags. The primary goal is to provide a community-driven, labeled set of addresses that can be used for research, analysis, and understanding the diverse types of entities in the IBC ecosystem.

## Schema

Each address entry has the following structure:

- **address**: The Cosmos address in a valid format.
- **label**: A descriptive label for the address.
- **tags**: Additional key-value pairs related to the address, such as the chain, protocol, contributor and type.


## Example

```json
{
  "address": "0x1234567890abcdef1234567890abcdef12345678",
  "label": "Coinbase Cold Wallet 1",
  "tags": {
    "chain": "osmosis",
    "org": "coinbase",
    "contributor": "Alice"
  }
}
```

## Networks

We currently support the following blockchains:

- Osmosis
- Cosmos Hub
- Neutron
- Terra

If you want to have your chain or protocol supported, please submit a pull request or open an issue.


## Labels and Tags

| Label             | Description                                      | Example Tags               |
|-------------------|--------------------------------------------------|----------------------------|
| Apollo Multisig   | An address owned by a cryptocurrency exchange.   | `chain: osmosis, protocol: apollo dao, type: contract` |
| Validatooor Reward Address    | Address used by Validatooor as reward address | `chain: cosmos-hub, org: validatooor, type: account` |
| Staking Contract  | An address where funds are staked for rewards.   | `chain: neutron, protocol: lido` |
| Bob Hacker Wallet 1   | Hacker wallet involved in phishing scam     | `chain: osmosis, type: account` |


## Contributing

We welcome community contributions! If you have a labeled Ethereum address or corrections to existing data, please submit a pull request or open an issue.

## License

This dataset is released under MIT Licence.
