<div align="center">
<a href="https://github.com/nantang-dao">
</a>

<h1 align="center">社区数字身份 (Community Digital Identity)</h1>

<p align="center">
<strong>中文</strong> · <a href="./README_EN.md">English</a>
</p>

<p align="center">
<strong>一套面向生态社区、乡村建设组织和社区成员的数字身份与协作系统</strong>
<br />
连接成员身份、社区协作与真实贡献，让每一次社区参与都能被记录、验证和认可
</p>

<p align="center">
<a href="https://semi.ntdao.xyz/"><strong>登录数字钱包 (Semi) »</strong></a>
<a href="https://bai.ntdao.xyz/"><strong>进入社区助手 (Bai) 
</p>

<p align="center">
<img src="https://img.shields.io/badge/Network-Optimism-red.svg" alt="Network">
<img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="License">
<img src="https://img.shields.io/badge/Status-Active_Dev-green.svg" alt="Status">
<img src="https://img.shields.io/badge/Account_Abstraction-ERC4337-orange.svg" alt="ERC-4337">
</p>
</div>

## 📖 项目简介

项目以 **Semi** 作为社区成员的数字身份入口，以 **Bai** 作为社区协作的记录平台，连接社区任务、协作、贡献审核与激励。

社区成员无需理解钱包、Gas、私钥或助记词等区块链知识，只需使用手机号或邮箱登录，即可进入社区、参与协作并积累自己的贡献记录。

系统通过区块链记录和验证贡献，为社区治理、成员激励与权益分配提供可信依据。

---

## 🌱 核心理念

### 真实社区优先

社区数字身份首先服务于真实的人和真实的社区关系。

### 贡献先于激励

社区积分和数字凭证应当建立在真实贡献之上。

### 社区共同制定规则

技术负责执行和记录，不能代替社区成员之间的讨论、协商和信任，不同社区可以根据自己的文化、规模和治理方式，制定适合自己的规则。

### 数据主权

社区运营数据产生的分析结果应当优先服务于社区，成员应当知道哪些信息会被收集、由谁查看、用于什么目的以及保留多长时间。

---

## 🧩 核心产品

### 社区数字身份（Semi）
**Semi** 为社区成员提供统一、低门槛的数字身份账户。成员可以通过手机号或邮箱登录，在无需管理助记词的情况下创建基于 Safe 的智能合约账户，并使用同一身份访问不同的社区应用。

#### Semi 的核心能力

- 手机号和邮箱登录
- 社区统一身份认证
- Safe 智能合约账户
- Gas 费用代付
- 社区积分和数字资产管理
- NFT/SBT 查看与管理
- 交易和权益记录
- Safe 多签安全机制
- 社区应用 OAuth 登录
- 第三方社区应用身份接入

### 社区协作助手（Bai）

**Bai** 是面向社区组织者和成员的协作平台。社区组织者可以通过 Bai 管理成员、发布任务、审核贡献和发放激励；社区成员可以领取任务、参与活动、提交凭证，并查看自己的参与记录和社区奖励。

#### Bai 的核心能力

- 社区创建与成员管理
- 成员角色和权限管理
- 单人及多人任务
- 任务发布、领取和协作
- 任务提交和审核
- 社区积分发放
- 成员贡献记录
- 社区参与和协作数据统计
- Semi 数字身份统一登录

---

## 🗺️ 路线图

### ✅ 已完成 (Completed)

- **Phase 1: 基础设施搭建 (2025.04 - 2025.10)**
    - [x]  确立 ERC-4337 架构与 Safe 合约集成。
    - [x]  实现手机号 (腾讯云 SMS) 注册与登录。
    - [x]  钱包基础功能：生成、导入导出、余额查询。
- **Phase 2: 智能合约与经济模型 (2025.11 - 2025.12)**
    - [x]  **积分系统**: ERC-20 合约部署与 Alchemy 索引集成。
    - [x]  **Gas 代付**: 集成 ZeroDev Paymaster。
    - [x]  **NFT/SBT**: 上线 NFT 展示。
    - [x]  增加邮箱登录支持。
- **Phase 3: 社区助手与生态互通 (2026.01 - 2026.02)**
    - [x]  **社区助手 MVP**: 用户管理面板与任务系统上线。
    - [x]  **OAuth 互通**: 完成 Wallet 与 Assistant 的单点登录。
    - [x]  **交易备注**: 支持链上转账附带可见性控制的备注信息。
    - [x]  部署国内加速代理 (SAS) 优化访问体验。

### 🚧 进行中 (Work in Progress)

- [ ]  **任务凭证上链**: 将任务完成记录铸造为 NFT/SBT。
- [ ]  **自动化激励**: 完善审核后的积分自动空投机制。
- [ ]  **移动端适配**: 调研小程序或 PWA 方案。

---

## 🛠 技术栈

| 领域 | 技术选型 |
| --- | --- |
| **前端 (Frontend)** | React, Next.js, TailwindCSS, ethers.js/viem |
| **后端 (Backend)** | Node.js, Supabase, OAuth 2.0 |
| **区块链 (Blockchain)** | Solidity, Hardhat, **ERC-4337**, **Safe Contracts** |
| **基础设施 (Infra)** | **Optimism (L2)**, **Alchemy** (Indexer), **ZeroDev** (Bundler/Paymaster) |
| **服务 (Services)** | Tencent Cloud (SMS) |

---

## 🚀 快速开始 (Getting Started)

### 环境依赖

- Node.js >= 18.0.0
- pnpm (推荐)

### 安装步骤

1. **克隆仓库**
    
    ```bash
    git clone [<https://github.com/nantang-dao/semi> app.git](<https://github.com/nantang-dao/Bai.git>)
    cd semi-app/cd Bai
    ```
    
2. **安装依赖**
    
    ```bash
    pnpm install
    ```
    
3. **配置环境变量**
复制 `.env.example` 为 `.env` 并填入 API Keys (Alchemy, ZeroDev, Tencent SMS 等)。
    
    ```bash
    cp .env.example .env
    ```
    
4. **启动开发环境**
    
    ```bash
    # 启动 Semi 钱包
    pnpm run dev:wallet
    
    # 启动社区助手
    pnpm run dev:assistant
    ```
---

## 👥 贡献者 (Contributors)

详细社区维护制度请参考：[CONTRIBUTING.md](https://github.com/nantang-dao/management/blob/main/CONTRIBUTING.md)

---

## 社区与联系

- 微信群：添加 xhy1120_ 备注 “乡建开发”

---

## 📜 许可证 (License)

本项目采用 [MIT License](https://www.notion.so/LICENSE) 开源。
