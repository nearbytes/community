# Nearbytes: a data-centric friend-to-friend decentralised storage and communication infrastructure
This repository is a entry point for the Nearbytes project. If intersted, please star this project and follow for updates, or open an issue to this repository for discussing ideas.

If you want to know more details, take a look at our [whitepaper](https://github.com/nearbytes/whitepaper) or [whitepaper-extended](./nearbytes-whitepaper-v0.1.pdf), or watch our webpage:

https://nearbytes.github.io/nearbytes/

The proof of concept app is available here: https://github.com/nearbytes/nearbytes-app and the specs (evovling) are at https://github.com/nearbytes/nearbytes-specs

## What

Nearbytes is a **local-first, friend-to-friend architecture** for persistent encrypted data spaces.
It separates:
- **Storage**: immutable encrypted blocks, addressable and verifiable by hash
- **State**: signed append-only events, replayed to reconstruct current files, chat, profiles, and app data

The same hub can be reopened across devices and storage locations without depending on a central always-online service.


## Goal

Make private collaboration and backup feel natural by providing an open protocol and usable app that:
- Keeps users in control of data and keys
- Avoids platform lock-in and single-service dependency
- Makes replication, sync, and recovery data-driven and verifiable

## What this project does

- Uses immutable encrypted blocks as the durable storage substrate
- Uses secret-derived hub identity and signatures for authenticated history
- Reconstructs current state by replaying signed events (instead of mutating storage in place)
- Supports transport-agnostic synchronization (local network, shared folders, removable media, cloud-backed folders, and more)
- Enables friend-to-friend replication where peers can store opaque bytes without controlling hub authority
- Keeps protocol and implementation open and inspectable

## Goals
- **Continuity across devices:** reopen the same hub wherever encrypted data and history are available.
- **Resilience by redundancy:** backup emerges from replication, not from one provider or one session staying online.
- **Collaboration without lock-in:** sharing depends on trusted relationships and data validity, not platform membership.
- **Auditability and recovery:** append-only signed history makes changes inspectable and replayable.

## How to get involved

- Watch this repository for updates.
- Open issues for feedback, use cases, and design discussion.
- Contribute via pull requests to docs, prototypes, and tooling.

## Roadmap highlights

- Evolve the desktop app, smartphone app, and core specifications in parallel
- Expand hub projections (files, chat, profiles, and additional app protocols)
- Improve sync, replay performance, and storage interoperability
- Publish clearer implementation, security, and integration documentation

## Contact

Have questions or want to contribute? Open an issue or a pull request and mention the maintainers, or write to vincenzoml at gmail dot com.
