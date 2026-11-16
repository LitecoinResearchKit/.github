<img src="logo.png" alt="Litecoin Research Kit" width="96" align="right" />

# Litecoin Research Kit

Tools to extract, explore and analyze the data stored in your Litecoin node,
MWEB included.

- **[Litview](https://litview.space)**: Litecoin's chain, read and measured.
  Live apps, thousands of charts, and every series as data. Free to use, no
  account needed.
- **[Litecoin Research Kit](https://litview.space/brk/)**: Rust crates for
  Litecoin Core data: RPC, block files in chain order, the live mempool,
  Litecoin's types and typed storage. Litview is built from all of them.

## Use it

- [Interactive API](https://litview.space/api) and [OpenAPI](https://litview.space/openapi.json)
- MCP endpoint: `https://mcp.litview.space/`
- [Developer guide](https://litview.space/dev/)

```bash
curl https://litview.space/api/series/count
```

## Self-host

Needs a Litecoin Core node with RPC and complete block files from genesis.

```bash
git clone https://github.com/LitecoinResearchKit/lrk && cd lrk
RUSTFLAGS="-C target-cpu=native" cargo install --locked --path crates/bitviewd --features litecoin --profile release-ltc
```

## Credits

A Litecoin fork of the [Bitcoin Research Kit](https://github.com/bitcoinresearchkit)
and [Bitview](https://bitview.space) by [nym21](https://x.com/_nym21_), MIT licensed.
