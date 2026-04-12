#  Aegis RWA Protocol

**Bridging real-world value with decentralized liquidity through compliant, institutional-grade tokenization on the Stellar network.**

[![Stellar](https://img.shields.io/badge/Network-Stellar-black?style=flat-square&logo=stellar)](https://stellar.org)
[![Soroban](https://img.shields.io/badge/Smart_Contracts-Soroban-purple?style=flat-square)](https://soroban.stellar.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square)](https://opensource.org/licenses/MIT)

Welcome to the official GitHub organization for **Aegis RWA**. We are building the infrastructure required to compliantly tokenize Real-World Assets (RWAs)—such as fractional real estate, treasury bills, and private credit—bringing transparent, composable, and programmable liquidity to traditional finance.



##  Ecosystem Overview

The Aegis RWA Protocol is composed of three foundational pillars, designed for maximum composability and developer experience.

*  **[`aegis-contracts`](https://github.com/AegisRWA/aegis-contracts)**: The core Soroban smart contracts written in Rust. Handles asset minting, KYC/whitelist compliance enforcement, and yield distribution.
*  **[`aegis-sdk`](https://github.com/AegisRWA/aegis-sdk)**: The official TypeScript middleware. Abstracts complex Stellar RPC interactions and XDR parsing, allowing developers to integrate Aegis RWA into any Node.js or browser environment seamlessly.
*  **[`aegis-dashboard`](https://github.com/AegisRWA/aegis-dashboard)**: The Next.js frontend reference implementation. Provides an institutional-grade interface for Administrators (minting/compliance) and Investors (portfolio tracking/transfers).


##  System Architecture

Our protocol enforces strict separation of concerns, ensuring compliance at the base layer while maximizing flexibility at the application layer.

```mermaid
graph TD
    A[Aegis Dashboard <br> Next.js / React] -->|RPC Calls / Wallet Signing| B(Aegis SDK <br> TypeScript)
    B -->|XDR / Transactions| C{Stellar RPC Node}
    C -->|Soroban Env| D[Aegis Contracts <br> Rust / WASM]
    
    subgraph Soroban Smart Contracts
    D --> E(Asset Minting)
    D --> F(Compliance & KYC)
    D --> G(Yield Distribution)
    end
    
    F -.->|Rejects non-whitelisted| E
```

## Protocol Roadmap

* Phase 1: Testnet MVP (Current) 
  * Deploy core Soroban contracts to Stellar Testnet.
  * Publish Alpha version of @aegis/sdk.
  * Release v1 of the Aegis Dashboard for community testing.
* Phase 2: Security & Audits
  * Comprehensive test coverage and formal verification. 
  * Third-party smart contract security audits. 
  * Integration with Stellar Ecosystem compliance oracles.
* Phase 3: Mainnet Launch
  * Deploy contracts to Stellar Public Network. 
  * Onboard initial institutional asset issuers. 
  * Launch developer grant program for SDK integrators.

## Getting Started
We welcome contributions from the global Web3 community! Whether you are a Rust veteran optimizing our Soroban logic, or a frontend engineer refining our dashboard, there is a place for you here.

1. Read our Contributing Guidelines to understand our workflow. 
2. Review our Code of Conduct. 
3. Check the Good First Issue labels on any of our repositories. 
4. Join the discussion in the Stellar Developer Discord.

Security Note: If you find a vulnerability, please DO NOT open a public issue. See our Security Policy for responsible disclosure.