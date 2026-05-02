# UniTrack4D
# UnityTrack 4D

Local desktop application for Store Scaler. Premium tier (Tier 2).

## What It Is

UnityTrack 4D is the visual interface for Store Scaler. It runs 100% locally on your machine. No cloud. No server connection. No data leaves your computer.

## Features

- One-click command execution (replaces terminal for non-technical users)
- Agentic view: see Claude Code working in real time
- Smart contract viewer: read StoreScalerVerifier and UniTrackPulse directly from the app
- Vault verification: auto-runs hash.sh on launch and compares against on-chain hash
- Pulse timeline: view your execution history from UniTrackPulse contract

## Architecture

UT4 connects to the internet for the same two things as the terminal tier:
1. Claude Code API calls to Anthropic (your key, your data)
2. Pulse transactions to Base blockchain (hook key, no API, random wallet + timestamp)

No other outbound connections. No MT server. Nothing else.

## Why the Source Code Is Public

So you can verify there are no hidden endpoints. Clone this repo, read the code, run a packet sniffer. Two destinations only: Anthropic API and Base RPC.

## No Commands Inside

UT4 is the interface, not the product. The commands live in StoreScaler_Private (the vault you purchased). UT4 reads them locally and executes through Claude Code. The IP never enters this repo.

## Requirements

- Store Scaler vault (StoreScaler_Private)
- Claude Max subscription or Anthropic API key
- macOS / Windows / Linux

## Links

- Protocol: github.com/MarketersTerminal/UniTrackProtocol
- Chain page: unitrackmt.org
- Product: marketersterminal.com
