<div align="center">
<a href="https://github.com/nantang-dao">
</a>

<h1 align="center">乡建数字身份 (Rural Digital Identity)</h1>

<p align="center">
<strong>链接城乡要素，赋能社区治理。</strong>
<br />
一套基于 ERC-4337 的数字身份与社区协作基础设施，专为生态社区设计。
</p>

<p align="center">
<a href="https://app.ntdao.xyz/"><strong>登录数字钱包 (Semi) »</strong></a>
·
<a href="https://bai.ntdao.xyz/"><strong>进入社区助手 (Bai) »</strong></a>
·
<a href="https://github.com/your-org/xiangjian-id/issues">报告 Bug</a>
</p>

<p align="center">
<img src="https://img.shields.io/badge/Network-Optimism-red.svg" alt="Network">
<img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="License">
<img src="https://img.shields.io/badge/Status-Active_Dev-green.svg" alt="Status">
<img src="https://img.shields.io/badge/Account_Abstraction-ERC4337-orange.svg" alt="ERC-4337">
</p>
</div>

## 📖 项目简介 (Introduction)

**“乡建数字身份”** 旨在利用 Web3 技术解决乡村建设中的组织与激励问题，构建 “数字乡民” 基础设施。通过 ERC - 4337 技术降低用户使用区块链门槛，借助社区助手打通链上贡献与现实权益，实现去中心化社区治理与激励。

本项目包含两个核心组件，实现了从“身份”到“协作”的闭环：

1. **Semi 钱包 (Semi-Custodial Wallet)**: 基于 ERC-4337 和 Safe 合约的网页钱包，支持社交登录与 Gas 代付，降低用户准入门槛。
2. **社区助手 (Community Assistant)**: 代号 "Bai"，一个集成了任务系统、用户管理与积分激励的社区治理中台。

---

## ✨ 核心特性 (Key Features)

### 🔐 Semi 钱包 (Identity & Assets)

| 功能 | 说明 |
| --- | --- |
| **便捷登录** | 支持手机号、邮箱登录，基于 ERC-4337 实现零门槛接入，无需助记词即可生成链上账户 |
| **托管安全** | 基于 **Safe** 智能合约账户，结合后端分片管理，平衡便捷与安全 |
| **资产管理** | 默认基于 Optimism 网络，支持 Gas 费代付，支持多链资产管理与切换 |
| **交易功能** | 交易历史查看、转账地址扫码、手机号转账等 |
| **徽章系统** | 展示 SBT 和 NFT，记录社区贡献与身份 |

### 🛠 社区助手 "Bai" (Collaboration & Governance)

| 功能 | 说明 |
| --- | --- |
| **社区管理** | 可视化展示成员活跃度与资产分布，实现用户管理 |
| **任务系统** | 结合乡建场景发布任务，支持单人/多人任务，实现任务领取、提交凭证、审核及积分自动发放 |
| **钱包连通** | 与数字钱包无缝连接，完成任务后自动验证并发放奖励 |
| **链上记录** | 支持上传凭证（图片/链接），将线下贡献转化为链上数据。 |

---

## 📅 演进与路线图 (History & Roadmap)

### 研发里程碑

### Semi 钱包

- 2025 年 4 月 15 日左右：项目调研、立项。
    - 里程碑 1（12000USD）：实现手机号登录、短信验证码发送、钱包身份管理、生成导入导出、查看余额及钱包授权 API 接口。
    - 里程碑 1 +（6500USD）：创建用户 Safe 合约、开发社区积分合约并集成、实现积分功能与转账、显示交易历史等多项功能扩展。完成产品功能验收、提供 API 文档并公开代码。
    - 里程碑 2（10875USD，2025 年 12 月 7 日交付）：开发 NFT/SBT 合约，部署用户专属 NFT 合约，实现 NFT 发放、转账、图片存储与链上索引，增加邮箱登录与用户名管理。
    - 2026 年 1 - 2 月：增加交易备注、积分交易接口、OAuth 登录及客户端配置，修复转账地址错误，增加用户名识别。

### 🛠 社区助手 "Bai"

- 第一阶段（3000USD，2025.12 - 2026.1.31）：
  实现手机号单点登录并绑定数字身份，用户可修改信息、查看钱包；完成任务系统闭环，实现积分发放并跳转数字钱包交易；进行多端测试、任务上链等。

### 路线图

### ✅ 已完成 (Completed)

- **Phase 1: 基础设施搭建 (2025.04 - 2025.10)**
    - [x]  确立 ERC-4337 架构与 Safe 合约集成。
    - [x]  实现手机号 (腾讯云 SMS) 注册与登录。
    - [x]  钱包基础功能：生成、导入导出、余额查询。
- **Phase 2: 智能合约与经济模型 (2025.11 - 2025.12)**
    - [x]  **积分系统**: ERC-20 合约部署与 Alchemy 索引集成。
    - [x]  **Gas 代付**: 集成 ZeroDev Paymaster。
    - [x]  **NFT/SBT**: 上线议事规则 NFT 展示与身份标识。
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

## 🛠 技术栈 (Tech Stack)【需修改】

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

## 项目管理规范

### 总体原则

开放协作：所有代码、文档、讨论尽可能公开，默认遵循开放透明的沟通方式。
轻量高效：流程简洁，强调贡献者自驱。
可持续性：鼓励更多人参与贡献，降低参与门槛，保障项目长期维护能力。
质量优先：确保提交内容满足基本质量标准，保持代码库干净、结构清晰。

### 数据库管理

由南塘 DAO 数字身份应用注册的用户，数据由南塘 DAO 开源小组拥有并管理。
未来其他社区使用数字身份且希望单独托管，在具备自托管能力的前提下，可使用自建数据库进行自托管，或获得数据备份。
使用 Supabase 云服务托管的 PostgreSQL 数据库，版本 v17 以上。

### 数据库安全

每周定期备份数据库 SQL，并妥善存储备份文件。
数据库账户妥善保存，仅 maintainer 可访问。
数据库账户和密码严禁写在文件代码中。

### 表结构原则

必须包含主键，尽量使用 Timestamp ID 生成 ID，以字符串格式存储。
字段建议具备明确的数据类型与长度，过长的可以使用 TEXT 存储可结构化数据，结构化数据可以用 JSONB 格式。
字段命名统一采用 snake_case。

---

## 👥 贡献者 (Contributors)

详细社区维护制度请参考：COMMUNITY_GUIDE.md

---

## 社区与联系

- 微信群：添加[微信号] 备注 “乡建开发”

---

## 📜 许可证 (License)

本项目采用 [MIT License](https://www.notion.so/LICENSE) 开源。
