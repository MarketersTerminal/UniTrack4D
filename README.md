# UniTrack4D

Desktop application for Store Scaler vault execution. Visual interface for Claude Code commands.

## What It Does

- Browse and execute vault commands through a GUI instead of CLI
- View on-chain verification status (reads StoreScalerVerifier contract)
- View pulse timeline (reads UniTrackPulse contract)
- Auto-verify vault hash on update

## Architecture

- 100% local application — no backend, no server, no data collection
- Reads commands from the local vault (same files Claude Code uses)
- Executes via Claude Code under the hood
- Reads contracts via ethers.js (Base RPC only)

## Source Code

This repo contains the full source code. Open for audit by anyone.
No commands are stored in this repo — commands live in the private vault (StoreScaler_Private).

## Links

- [Store Scaler](https://github.com/MarketersTerminal/StoreScaler) — the product
- [UniTrack Protocol](https://github.com/MarketersTerminal/UniTrackProtocol) — smart contracts
- [Marketers Terminal](https://github.com/MarketersTerminal/MarketersTerminal) — organization hub
- [unitrackmt.org](https://unitrackmt.org) — on-chain verification page
