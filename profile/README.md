# Meshifact

Meshifact is a decentralized artifact distribution system.

## Overview

Meshifact lets authorized devices share artifacts over a peer-to-peer network.

A device can:

* Publish an artifact
* Find an artifact
* Download an artifact
* Share an artifact with other devices

## Architecture

Meshifact has two main parts:

* Control plane
* Data plane

### Control plane
The control plane determines which devices can join the network and which artifacts they can access.

The control plane manages:

* User authentication
* Device authentication
* Device registration
* Access control
* Device revocation
* System policy



### Data plane
The data plane moves artifact data between devices.

The data plane provides:

* Peer discovery
* Artifact discovery
* Artifact transfer
* Local artifact storage
* Data verification

## Content Addressing
Meshifact uses content addressing for artifacts.

Each artifact has a content identifier.
The identifier represents the artifact content.

This provides:

* Content integrity
* Duplicate detection
* Reliable artifact identification

## Peer Network
Only authorized devices can join a Meshifact network.

Each device has a unique device identity.

The system can revoke a device when it is no longer allowed to use the network.

Artifact data moves between authorized peers.

## Technology
Meshifact uses:

* TypeScript
* Node.js
* libp2p
* Helia
* IPFS content addressing

## Project Structure

| Repository | Purpose                               |
| ---------- | ------------------------------------- |
| `node`     | Meshifact node and artifact functions |
| `daemon`   | Runs a Meshifact node as a service    |
| `cli`      | Command line interface                |
| `client`   | Desktop client                        |

## Project Status
Meshifact is under development.

The current development goals are:

* Peer discovery
* Artifact publishing
* Artifact discovery
* Artifact download
* Content verification
* Device authentication
* Access control
* Windows support
* Linux support
