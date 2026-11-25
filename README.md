# datocms-plugin-crypto-address-validator

Zero-dependency **DatoCMS plugin** and field extension (`datocms-plugin-sdk`) for validating multi-chain cryptocurrency wallet address syntax, cryptographic checksums, mandatory custodial **Memo / Destination Tag** routing identifiers, and prefix/suffix **vanity address-poisoning lookalike detection** across 46+ blockchain networks.

Built and maintained by the security engineering team behind the [AllSwap Multi-Chain Address & Memo Validator](https://allswap.io/tools/address-validator) and the [AllSwap Non-Custodial Cross-Chain Swap & Bridge Aggregator](https://allswap.io/).

## Features

- **DatoCMS String & JSON Field Addon (`cryptoAddressValidator`)**: Validate destination wallet addresses and custodial Memo / Destination Tag pairs directly inside DatoCMS content models before publishing treasury, grant, or payout records.
- **Multi-Chain Address Syntax & Checksum Validation**: Supports EVM (`0x...`), Bitcoin (Legacy, SegWit, Taproot Bech32m), Solana (Ed25519 Base58), XRP Ledger, Stellar (StrKey), Cosmos Hub (Bech32), TON, TRON, Sui, Aptos, Hedera, and EOSIO wallet addresses.
- **Mandatory Memo / Destination Tag Enforcement**: Prevents accidental custodial fund loss by enforcing required Destination Tags (`XRP`), Memos (`XLM`, `ATOM`, `HBAR`, `EOS`), and Comments (`TON`).
- **Vanity Address-Poisoning Defense**: Flags lookalike addresses that match the first 5 and last 4 characters of a known trusted reference address while differing in the middle bytes.

## Installation

Install via the **DatoCMS Plugins Marketplace** or npm:

```bash
npm install datocms-plugin-crypto-address-validator
```

## Documentation & Reference Links

- **Interactive Multi-Chain Address & Memo Validator**: [https://allswap.io/tools/address-validator](https://allswap.io/tools/address-validator)
- **AllSwap Cross-Chain Swap & Bridge Aggregator**: [https://allswap.io](https://allswap.io)
- **Technical Specification & Developer Docs**: [https://allswap.io/docs](https://allswap.io/docs)
- **Core CLI & Reproducible Test Suite (MIT)**: [https://github.com/zhangglnuo-art/multichain-memo-address-validator](https://github.com/zhangglnuo-art/multichain-memo-address-validator)

## License

MIT © [AllSwap Security Labs](https://allswap.io)
