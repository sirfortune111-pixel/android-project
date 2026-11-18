# Technical Specification & Agent Directives

## 1. Core Architecture
- Self-Custody: Local key generation & Android Keystore encryption. Zero server access to keys.
- Zero-KYC: Immediate onboarding without identity verification.
- Unified UX: Single interface for multi-currency assets and payment systems.
- Smart Routing 24/7: Real-time rate aggregation across liquidity providers for optimal swap execution.

## 2. Agent Directives

### DIRECTIVE 01 - SECURITY & SELF-CUSTODY
Act as a Principal FinTech & Cryptography Architect. Build a non-custodial multi-currency mobile wallet. Store private keys strictly client-side via Android Keystore. Never log or transmit keys/mnemonics.

### DIRECTIVE 02 - 24/7 SMART EXCHANGE ROUTER
Act as a Senior Backend Engineer. Aggregate live quotes 24/7, normalize fees/slippage, and return the best swap route in real time.

### DIRECTIVE 03 - UNIFIED MOBILE UX
Act as a Senior Mobile Developer. Consolidate multi-chain balances in one screen and execute swaps in 3 steps (Select Pair -> Best Rate -> Biometric Sign) without manual address copying.
