<div align="center">
  <a href="https://github.com/nantang-dao">
  </a>

  <h1 align="center">Community Digital Identity</h1>

  <p align="center">
    <strong>A digital identity and collaboration system for ecosystem communities, rural development organizations, and community members</strong>
    <br />
    Connecting member identity, community collaboration, and real-world contributions—so every act of participation can be recorded, verified, and recognized.
  </p>

  <p align="center">
    <a href="https://semi.ntdao.xyz/"><strong>Log in to Semi »</strong></a>
    &nbsp;&nbsp;
    <a href="https://bai.ntdao.xyz/"><strong>Open Bai
  </p>

  <p align="center">
    <img src="https://img.shields.io/badge/Network-Optimism-red.svg" alt="Network">
    <img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="License">
    <img src="https://img.shields.io/badge/Status-Active_Development-green.svg" alt="Status">
    <img src="https://img.shields.io/badge/Account_Abstraction-ERC--4337-orange.svg" alt="ERC-4337">
  </p>
</div>

## 📖 Overview

This project uses **Semi** as the digital identity gateway for community members and **Bai** as the platform for recording community collaboration. Together, they connect community tasks, collaboration, contribution reviews, and incentives.

Community members do not need to understand wallets, gas fees, private keys, or seed phrases. They can simply log in with a phone number or email address to join communities, participate in collaborative work, and build a verifiable contribution history.

The system records and verifies contributions on the blockchain, providing a trusted foundation for community governance, member incentives, and benefit distribution.

---

## 🌱 Core Principles

### Real Communities First

Community digital identity should serve real people and authentic community relationships.

### Contribution Before Incentives

Community points and digital credentials should be based on genuine contributions.

### Communities Define Their Own Rules

Technology is responsible for executing and recording rules, but it cannot replace discussion, coordination, and trust among community members. Each community can establish rules suited to its own culture, scale, and governance model.

### Data Sovereignty

Insights derived from community operational data should primarily serve the community itself. Members should know what information is collected, who can access it, how it is used, and how long it is retained.

---

## 🧩 Core Products

### Community Digital Identity — Semi

**Semi** provides community members with a unified and accessible digital identity account. Members can log in with a phone number or email address and create a Safe-based smart contract account without managing a seed phrase. The same identity can then be used across multiple community applications.

#### Key Features of Semi

- Phone number and email login
- Unified community identity authentication
- Safe smart contract accounts
- Sponsored gas fees
- Community points and digital asset management
- NFT and SBT viewing and management
- Transaction and entitlement history
- Safe multisignature security
- OAuth login for community applications
- Identity integration for third-party community applications

### Community Collaboration Assistant — Bai

**Bai** is a collaboration platform for community organizers and members. Organizers can use Bai to manage members, publish tasks, review contributions, and distribute incentives. Members can claim tasks, participate in activities, submit evidence of their work, and review their participation history and community rewards.

#### Key Features of Bai

- Community creation and member management
- Member roles and permissions
- Individual and collaborative tasks
- Task publishing, claiming, and collaboration
- Task submission and review
- Community point distribution
- Member contribution records
- Community participation and collaboration analytics
- Unified login through Semi

---

## 🗺️ Roadmap

### ✅ Completed

- **Phase 1: Infrastructure Setup (2025.04–2025.10)**
  - [x] Established the ERC-4337 architecture and integrated Safe contracts
  - [x] Implemented phone number registration and login using Tencent Cloud SMS
  - [x] Delivered core wallet features, including wallet creation, import and export, and balance queries

- **Phase 2: Smart Contracts and Economic Model (2025.11–2025.12)**
  - [x] **Point System:** Deployed ERC-20 contracts and integrated Alchemy indexing
  - [x] **Gas Sponsorship:** Integrated the ZeroDev Paymaster
  - [x] **NFT/SBT:** Added NFT display functionality
  - [x] Added support for email login

- **Phase 3: Community Assistant and Ecosystem Integration (2026.01–2026.02)**
  - [x] **Community Assistant MVP:** Launched the user management dashboard and task system
  - [x] **OAuth Integration:** Implemented single sign-on between Semi and Bai
  - [x] **Transaction Notes:** Added blockchain transaction notes with visibility controls
  - [x] Deployed a domestic acceleration proxy service to improve access performance

### 🚧 Work in Progress

- [ ] **On-chain Task Credentials:** Mint completed task records as NFTs or SBTs
- [ ] **Automated Incentives:** Improve automatic point distribution following contribution approval
- [ ] **Mobile Support:** Evaluate mini-program and PWA solutions

---

## 🛠 Technology Stack

| Area | Technologies |
| --- | --- |
| **Frontend** | React, Next.js, Tailwind CSS, ethers.js / viem |
| **Backend** | Node.js, Supabase, OAuth 2.0 |
| **Blockchain** | Solidity, Hardhat, **ERC-4337**, **Safe Contracts** |
| **Infrastructure** | **Optimism (L2)**, **Alchemy** (Indexer), **ZeroDev** (Bundler/Paymaster) |
| **Services** | Tencent Cloud SMS |

---

## 🚀 Getting Started

### Prerequisites

- Node.js 18.0.0 or later
- pnpm (recommended)

### Installation

#### 1. Clone the repositories

**Semi**

```bash
git clone https://github.com/nantang-dao/semi.git
cd semi
```

**Bai**

```bash
git clone https://github.com/nantang-dao/Bai.git
cd Bai
```

#### 2. Install dependencies

Run the following command inside the relevant project directory:

```bash
pnpm install
```

#### 3. Configure environment variables

Copy `.env.example` to `.env`, then provide the required API keys and credentials, including Alchemy, ZeroDev, and Tencent Cloud SMS.

```bash
cp .env.example .env
```

#### 4. Start the development environment

Start Semi:

```bash
pnpm run dev:wallet
```

Start Bai:

```bash
pnpm run dev:assistant
```

---

## 👥 Contributors

For details about the community maintenance and contribution process, see [CONTRIBUTING.md](https://github.com/nantang-dao/management/blob/main/CONTRIBUTING.md).

---

## Community and Contact

- **WeChat group:** Add `xhy1120_` and include “乡建开发” in your friend request.

---

## 📜 License

This project is licensed under the [MIT License](https://github.com/nantang-dao/management/blob/main/LICENSE).
