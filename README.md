<div align="center">

# 🔒 Siphon Protocol

[![Next.js](https://img.shields.io/badge/Next.js-14-black?style=for-the-badge&logo=next.js)](https://nextjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.0-blue?style=for-the-badge&logo=typescript)](https://www.typescriptlang.org/)
[![Three.js](https://img.shields.io/badge/Three.js-0.180-green?style=for-the-badge&logo=three.js)](https://threejs.org/)
[![Rust](https://img.shields.io/badge/Rust-1.70-orange?style=for-the-badge&logo=rust)](https://www.rust-lang.org/)
[![Solidity](https://img.shields.io/badge/Solidity-0.8.20-black?style=for-the-badge&logo=solidity)](https://soliditylang.org/)
[![Citcom](https://img.shields.io/badge/Citcom-latest-blue?style=for-the-badge)](https://github.com/citcomsuite/citcoms)
[![Python](https://img.shields.io/badge/Python-3.11-blue?style=for-the-badge&logo=python)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)](LICENSE)

**Enabling untraceable, hyperliquid and institutional-grade DeFi privacy with Fully Homomorphic Encryption and Zero-Knowledge proofs.**


[🚀 Live Demo](https://siphon-eth.vercel.app) 

---

</div>

## 🎯 The Problem We Solve

### ⚠️ Three Critical Privacy Crises in DeFi:

<table>
<tr>
<td width="33%">


#### 🔍 **Wallets Are Tracked**
- **Every transaction** exposes your entire financial history
- **Portfolio strategies** are visible to competitors and regulators
- **Institutional traders** cannot operate with confidentiality

</td>
<td width="33%">

#### 🤖 **Value is Extracted**
- **Order intent** leaks milliseconds before execution
- **Visible flow**  widens quotes and worsens fills.
- **Sniping and MEV**  extraction destroys profitability.

</td>
<td width="33%">

#### 💰 **The Privacy-Liquidity Dilemma**
- **Privacy coins** (ZEC, XMR) lack DeFi integration
- **Dark pools** are fragmented and underutilized
- **Users forced** to choose: privacy OR best execution

</td>
</tr>
</table>

### 📊 Market Reality
- **$280M** lost monthly to front-running attacks on DEXs 
- **$12B** in privacy coin market cap lacks DeFi integration
- **Zero** truly private DEXs with easy access to global liquidity


---

## 🚀 The Siphon Solution

<div align="center">

### 🌉 **The Privacy Bridge**

**Siphon serves as the seamless privacy-preserving gateway between public and private capital, facilitating secure, private and verifiable movement of assets across multiple blockchains. By enabling frictionless access to the deepest, most liquid DeFi opportunities in a true omnichain environment, Siphon empowers institutions and individuals alike to transact and deploy strategies at scale—without sacrificing confidentiality, competitive edge, or market efficiency.**
</div>

### ✨ Key Features:

<table>
<tr>
<td width="50%">

#### 🔒 **Complete Privacy**
- Portfolio, PnL, and strategies are no longer visible on-chain
- Encrypted state management

#### ⚡ **No Front-running**
- Eliminates order sniffing and MEV extraction
- Private transaction routing

</td>
<td width="50%">

#### 💰 **Better Pricing**
- Cheaper transaction prices through optimized execution
- Reduced slippage through privacy-preserving routing

#### 🌐 **Omnichain**
- Hyperliquid execution across multiple chains
- Privacy preserved end-to-end

</td>
</tr>
</table>

<img src="https://github.com/undefinedlab/siphon_eth/blob/master/docs/4.png" alt="Siphon Architecture Diagram" width="100%" />


---

## 🛠️ Technical Architecture

### 🔧 Core Technologies:

<table>
<tr>
<td width="25%" align="center">

#### 🔐 **FHE**
**Fully Homomorphic Encryption**
Enables computation on encrypted data

</td>
<td width="25%" align="center">

#### 🎭 **ZK Proofs**
**Zero-Knowledge Proofs**
Cryptographic assurance without revealing data

</td>
<td width="25%" align="center">

#### 🌉 **Avail Nexus SDK**
**Cross-Chain Operations**  
Seamless multi-chain execution

</td>
<td width="25%" align="center">

#### 📈 **Pyth Network**
**Price Feeds & Randomness**  
Reliable price oracles and random number generation

</td>
<td width="25%" align="center">

#### 🛠️ **Hardhat**
**Deployment Tool**  
Flexible, developer-friendly smart contract deployment

</td>
</tr>
</table>


### The Five-Layer Architecture:

```
┌─────────────────────────────────────────────────────────────┐
│ Layer 5: Liquidity Interface                                │
│ - Public DEX aggregators                                     │
│ - Cross-chain bridges                                        │
│ - Modular design for privacy-native assets                   │
└─────────────────────────────────────────────────────────────┘
┌─────────────────────────────────────────────────────────────┐
│ Layer 4: Verification & Settlement                          │
│ - ZK proof of correct execution                             │
│ - On-chain verification                                      │
│ - Cryptographic guarantees                                    │
└─────────────────────────────────────────────────────────────┘
┌─────────────────────────────────────────────────────────────┐
│ Layer 3: Confidential Execution Environment (FHE Engine)    │
│ - Encrypted mempool                                          │
│ - Computation on encrypted data                              │
│ - Order matching & slippage calculation                      │
└─────────────────────────────────────────────────────────────┘
┌─────────────────────────────────────────────────────────────┐
│ Layer 2: Shielded Pool                                       │
│ - Incremental Merkle trees                                   │
│ - Zero-knowledge membership proofs                           │
│ - Nullifier system for double-spend prevention               │
└─────────────────────────────────────────────────────────────┘
┌─────────────────────────────────────────────────────────────┐
│ Layer 1: Vault Contract                                      │
│ - Trustless escrow for public assets                         │
│ - ETH, USDC, WBTC and more                                   │
│ - Release on valid ZK proof verification                     │
└─────────────────────────────────────────────────────────────┘
```

## 📁 Project Structure
```
siphon/
├── 📂 circuits/              # ZK-SNARK circuits for private proofs
│
├── 📂 contracts/             # Solidity smart contracts for on-chain logic

├── 📂 docs/                  # Documentation

├── 📂 packages/              # Reusable cryptographic and utility packages
│   ├── fhe-lib/
│   ├── zk-proofs/
│   └── crypto-utils/
│
├── 📂 public/                # Static assets

├── 📂 src/                   # Application source code
│   ├── 📂 app/              # Next.js 14 App Router pages and API routes
│   ├── 📂 components/       # Reusable React components
│   │   ├── ui/
│   │   ├── trading/
│   │   └── wallet/
│   │
│   ├── 📂 lib/              # Core FHE and ZK proof implementations
│   │   ├── fhe/
│   │   ├── zk/
│   │   └── blockchain/
│   │
│   ├── 📂 hooks/            # React hooks
│   ├── 📂 utils/            # Utility functions
│   └── 📂 types/            # TypeScript types
│
├── 📄 README.md


```




## 🚀 Quick Start

### 📋 Prerequisites

- **Node.js** 18+ 
- **npm** or **yarn**
- **Git**

### ⚡ Installation

```bash
# Clone the repository
git clone https://github.com/undefinedlab/siphon_eth.git
cd siphon_eth/siphon

# Install dependencies
npm install

# Run development server
npm run dev
```

🌐 Open [http://localhost:3000](http://localhost:3000) to see the application.

### 📜 Available Scripts

| Command | Description |
|---------|-------------|
| `npm run dev` | 🚀 Start development server |
| `npm run build` | 🏗️ Build for production |
| `npm run start` | ▶️ Start production server |
| `npm run lint` | 🔍 Run ESLint |
| `npm run test` | 🧪 Run tests |


---

## 🤝 Contributing

We welcome contributions! Here's how you can help:

### 🚀 Getting Started

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/amazing-feature`)
3. **Commit** your changes (`git commit -m 'Add amazing feature'`)
4. **Push** to the branch (`git push origin feature/amazing-feature`)
5. **Open** a Pull Request

### 📋 Development Guidelines

- Follow the existing code style
- Add tests for new features
- Update documentation as needed
- Ensure all tests pass

---

## 📄 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

---


## ⚠️ Disclaimer

> **This software is in active development and should be used for testing purposes only. Always conduct your own research and never invest more than you can afford to lose.**

---

<div align="center">

### 🌟 **Siphon Protocol**


**Made with ❤️ for Eth Global **

</div>
