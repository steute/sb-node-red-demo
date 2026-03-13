# CLAUDE.md — sb-node-red-demo

Shared conventions (language, terminology, proofreading) are defined in the parent workspace `CLAUDE.md`.

## Project Overview

Example Node-RED project demonstrating how to receive and process live data from the steute Sensor Bridge via HTTP notifications. Intended as a starting point for users building their own integrations.

## How It Works

- A single Node-RED flow listens for HTTP POST requests on `/nodered/notifications`.
- The Sensor Bridge is configured to send event notifications (switch events, battery state, RSSI, etc.) to this endpoint.
- Debug nodes display incoming payloads for inspection.

## Usage

See `REAMDME.md` for setup and usage instructions.

## Key Files

- **`flows.json`** — The Node-RED flow definition.
- **`flows_cred.json`** — Encrypted credentials (if any).
- **`package.json`** — Node-RED project metadata.
