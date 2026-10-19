# Nearbytes

**A local-first, friend-to-friend architecture for persistent, encrypted, collaborative data spaces.**

This repository is the entry point of the Nearbytes project: star or watch it to follow updates, and open an issue to discuss ideas, use cases or design.

| | |
|---|---|
| Website | https://nearbytes.github.io/nearbytes/ |
| Paper | *Local-first Coordination via Friend-to-Friend Choreographies*, Journal of Logical and Algebraic Methods in Programming, 2026 — [doi:10.1016/j.jlamp.2026.101190](https://doi.org/10.1016/j.jlamp.2026.101190) |
| Whitepaper | [nearbytes/whitepaper](https://github.com/nearbytes/whitepaper) · [extended version (PDF)](./nearbytes-whitepaper-v0.1.pdf) |
| App (proof of concept) | [nearbytes/nearbytes-app](https://github.com/nearbytes/nearbytes-app) |
| Specifications (evolving) | [nearbytes/nearbytes-specs](https://github.com/nearbytes/nearbytes-specs) |

## The idea

Nearbytes separates two things that most systems keep together:

- **Storage** — immutable encrypted blocks, addressed and verified by their hash.
- **State** — signed, append-only events, replayed to reconstruct current files, chat, profiles and application data.

Because state is rebuilt from data rather than held by a server, the same *hub* can be reopened on any device and from any storage location where its encrypted blocks and history are available. No central, always-online service is required.

## What it does

- Uses immutable encrypted blocks as the durable storage substrate.
- Derives hub identity from a secret and signs history, so every change is authenticated.
- Reconstructs state by replaying signed events instead of mutating storage in place.
- Synchronises over any transport: local network, shared folders, removable media, cloud-backed folders and more.
- Lets friends replicate each other's data as opaque bytes, without gaining any authority over the hub.
- Keeps protocol and implementation open and inspectable.

## Goals

- **Continuity across devices** — reopen the same hub wherever its data and history are.
- **Resilience by redundancy** — backup emerges from replication, not from one provider staying online.
- **Collaboration without lock-in** — sharing rests on trusted relationships and valid data, not on platform membership.
- **Auditability and recovery** — append-only signed history makes every change inspectable and replayable.
- **Users in control** of their data and keys.

## Roadmap

- Evolve the desktop app, the smartphone app and the core specifications in parallel.
- Add hub projections: files, chat, profiles, and further application protocols.
- Improve sync, replay performance and storage interoperability.
- Publish implementation, security and integration documentation.

## Get involved

- **Watch** this repository for updates.
- **Open an issue** for feedback, use cases and design discussion.
- **Send a pull request** to docs, prototypes and tooling.

Questions? Open an issue and mention the maintainers, or write to vincenzoml at gmail dot com.
