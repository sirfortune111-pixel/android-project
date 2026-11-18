# Техническое задание: Мультивалютный Non-Custodial Exchange-кошелёк

## 1. Архитектурные инварианты
- **Self-Custody:** Приватные ключи и seed-фразы генерируются, шифруются (Android Keystore / AES-256) и хранятся строго локально на устройстве. Сервер не имеет доступа к средствам пользователя.
- **Zero-KYC:** Отсутствие обязательной верификации личности для хранения и криптографических операций.
- **Unified UX:** Единый интерфейс для управления разными активами и платёжными системами без необходимости устанавливать отдельные приложения.
- **Smart Routing 24/7:** Автоматический анализ котировок множества обменных провайдеров в реальном времени и исполнение обмена по лучшему курсу в несколько кликов.

## 2. Директивные команды для AI-агентов

### DIRECTIVE 01 — SYSTEM ARCHITECTURE & SECURITY
Act as a Principal FinTech & Cryptography Architect. Design a non-custodial multi-currency mobile wallet with an integrated real-time exchange aggregator.
- Never transmit, log, or store user private keys or mnemonics on any backend server. All transaction signing must execute strictly client-side.
- Implement No-KYC onboarding: immediate access upon local wallet creation/import.
- Enforce hardware-backed encryption (Android Keystore) for local key storage.

### DIRECTIVE 02 — REAL-TIME SMART EXCHANGE ROUTER (24/7)
Act as a Senior Backend & Quantitative Systems Engineer. Build a quote aggregation service that:
- Streams and polls live exchange rates across multiple liquidity providers 24/7.
- Normalizes fees, spreads, and slippage in real time.
- Returns the single optimal execution route for any pair (Asset_A -> Asset_B) at the moment of swap initiation.

### DIRECTIVE 03 — UNIFIED MOBILE CLIENT & UX FLOW
Act as a Senior Mobile Developer. Implement a unified interface that eliminates multi-app fragmentation:
- Consolidate multi-chain balances into a single portfolio screen.
- Reduce asset conversion to a 3-step flow: Select Pair & Amount -> Review Best Smart-Routed Rate -> Biometric Sign & Execute.
- Eliminate manual address copying during swaps to prevent user errors and fund loss.
