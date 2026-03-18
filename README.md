# ZipherPunk — Cypherpunk Privacy Tools for Zclassic

**Privacy advocacy, wallet development, and post-quantum cryptographic research for [Zclassic (ZCL)](https://zclassic.org).**

Built by [@VicThor2013](https://x.com/VicThor2013) with [Claude](https://claude.ai) (Anthropic).

Website: **[zipherpunk.com](https://zipherpunk.com)**

---

## What is ZipherPunk?

ZipherPunk is a cypherpunk project building privacy-first tools for the Zclassic cryptocurrency ecosystem. Zclassic is a fork of Zcash that removes the 20% founder's reward — 100% of block rewards go to miners. Same zk-SNARK privacy, zero corporate interests.

## Projects

### ZipherX — Shielded-Only Wallet (macOS / iOS)

Privacy-absolute Zclassic wallet. Shielded transactions only (z-to-z). No transparent addresses. No trusted servers.

- **Secure Enclave** hardware key protection (iPhone 8+, Apple Silicon)
- **Embedded Tor** via Arti router with .onion hidden service
- **Local Sapling zk-SNARK proofs** generated on-device (~30 seconds)
- **Multi-peer consensus** — 8+ peers, 5/8 Byzantine fault tolerance
- **Encrypted P2P chat** over Tor with in-chat payments
- **Full Node mode** — embedded zclassicd for complete blockchain verification (macOS)
- **Biometric auth** — Face ID / Touch ID with auto-lock
- **BIP-39** 24-word seed recovery
- Swift + Rust, ~87,000 lines of code

**Download:** [GitHub Releases](https://github.com/ZipherPunk/ZipherX/releases/latest) | **Source:** [github.com/ZipherPunk/ZipherX](https://github.com/ZipherPunk/ZipherX)
**iOS Beta:** [TestFlight](https://testflight.apple.com/join/ZCzZRdaZ)

### ZipherX Multi — Cross-Platform Wallet (Android / macOS / Linux / Windows / iOS)

Multi-platform Zclassic wallet supporting both transparent and shielded (Sapling) transactions. Rust core with native UIs everywhere. No Electron.

- **Sapling shielded transactions** — full zk-SNARK privacy
- **Native desktop** (egui) — single Rust binary, no JVM
- **Android** — Material 3 / Jetpack Compose with biometric auth
- **Direct P2P networking** — connects to Zclassic nodes directly
- **Tor built-in** — optional onion routing for network privacy
- **Secure storage** — Argon2id + AES-256-GCM encrypted wallet data
- **BIP-39** 24-word seed recovery
- **Fast sync** via boost files

**Download:** [GitHub Releases](https://github.com/ZipherPunk/zipherx_multi/releases/latest) | **Source:** [github.com/ZipherPunk/zipherx_multi](https://github.com/ZipherPunk/zipherx_multi)

### Zclassic Quantum Threat Analysis

Comprehensive quantum computing threat analysis auditing every cryptographic primitive in Zclassic across all protocol layers — transparent, Sapling, Sprout, Proof-of-Work, and network — against Shor's and Grover's algorithms.

- **12 out of 18 primitives** are BROKEN by quantum computers
- **6 out of 9 Sapling primitives** are vulnerable (including Groth16, Pedersen, Curve25519 ECDH)
- **Post-quantum replacement map** — ML-DSA-65, STARKs, ML-KEM-768, SHA3-256 (per NIST FIPS 203/204/205)
- **5-phase strategic migration roadmap**
- **"Harvest now, decrypt later"** — passive attacks can deanonymize historical shielded transactions

**Read:** [zipherpunk.com/zclassic-quantum-analysis.html](https://zipherpunk.com/zclassic-quantum-analysis.html)

## Why Zclassic?

- **No Founder's Reward** — 100% of block rewards go to miners
- **zk-SNARK Privacy** — Groth16 zero-knowledge proofs hide sender, receiver, and amount
- **Decentralized** — no company, no foundation, community-driven
- **Battle-tested** — based on Zcash protocol, years of cryptographic research
- **Censorship resistant** — no one can stop your transaction or freeze your funds

## Links

| | |
|---|---|
| **Website** | [zipherpunk.com](https://zipherpunk.com) |
| **X / Twitter** | [@VicThor2013](https://x.com/VicThor2013) · [@ZipherPunk](https://x.com/ZipherPunk) |
| **GitHub** | [github.com/ZipherPunk](https://github.com/ZipherPunk) |
| **ZipherX Source** | [github.com/ZipherPunk/ZipherX](https://github.com/ZipherPunk/ZipherX) |
| **ZipherX Multi Source** | [github.com/ZipherPunk/zipherx_multi](https://github.com/ZipherPunk/zipherx_multi) |
| **Zclassic** | [zclassic.org](https://zclassic.org) |

## Important Disclaimers

### Educational Purpose Only

All content on this site, including cryptographic analyses, technical reports, and security assessments, is provided **strictly for educational and informational purposes**. Nothing constitutes financial, investment, or trading advice, or professional security consulting.

### No Warranty

Technical content is AI-assisted, **may contain errors, inaccuracies, or outdated information**, and has **not been formally peer-reviewed** or audited by a certified third party. The Quantum Threat Analysis is an independent educational research document, **not** a professional security audit.

### Limitation of Liability

The authors **accept no responsibility or liability** for any loss, damage, or consequence arising from use of this information, including financial losses, security incidents, or decisions based on technical content.

### Cryptocurrency Risk

Cryptocurrency is inherently risky. Zclassic (ZCL) may lose all value. Always do your own research (DYOR).

## License

[MIT License](LICENSE)

## Contributing

Contributions, corrections, and peer review welcome. Open an issue or submit a pull request.
