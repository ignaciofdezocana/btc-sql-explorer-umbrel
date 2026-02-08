# BTC SQL Explorer - Umbrel Community App Store

Run SQL queries against your Bitcoin full node's blockchain data, directly from your Umbrel.

## What is BTC SQL Explorer?

BTC SQL Explorer syncs blocks, transactions, inputs, and outputs from your Bitcoin Core node into a local DuckDB database and provides a modern web UI with:

- CodeMirror SQL editor with syntax highlighting
- Results table with sorting and pagination
- Interactive charts (bar, line, scatter, area, pie)
- CSV export
- Library of example queries to get started
- Saved queries

Your data never leaves your device.

## Install on your Umbrel

1. Open your Umbrel dashboard
2. Go to **App Store** > **Community App Stores**
3. Add this repository URL:

```
https://github.com/ignaciofdezocana/btc-sql-explorer-umbrel
```

4. Find **BTC SQL Explorer** in the App Store and click **Install**

## Requirements

- An Umbrel Home (or any device running umbrelOS)
- **Bitcoin Node** app installed and fully synced

## How it works

Once installed, BTC SQL Explorer automatically connects to your Umbrel's Bitcoin Core node via local RPC. A background sync process continuously ingests new blocks into a DuckDB database stored on your device. The web UI is accessible from your Umbrel dashboard.

Initial sync will take some time depending on how many blocks your node has. Progress is shown in the app logs.

## Source Code

- **App**: [github.com/ignaciofdezocana/btc-sql-explorer](https://github.com/ignaciofdezocana/btc-sql-explorer)
- **Umbrel packaging**: [github.com/ignaciofdezocana/btc-sql-explorer-umbrel](https://github.com/ignaciofdezocana/btc-sql-explorer-umbrel)
