# 贡献指南 (Contributing Guide)

欢迎您参与“乡建数字身份”开源社区的建设！本指南旨在帮助您了解如何有效地为项目做出贡献，确保我们的协作过程高效、顺畅。

## 一、总体原则
1. **开放协作**：所有代码、文档、讨论尽可能公开，默认遵循开放透明的沟通方式。
2. **轻量高效**：流程简洁，强调贡献者自驱。
3. **可持续性**：鼓励更多人参与贡献，降低参与门槛，保障项目长期维护能力。
4. **质量优先**：确保提交内容满足基本质量标准，保持代码库干净、结构清晰。
## 二、代码仓库
本项目的代码仓库位于：[https://github.com/nantang-dao](https://github.com/nantang-dao)
### 数字钱包
 - **前端代码 (Semi App)**：[https://github.com/nantang-dao/semi-app](https://github.com/nantang-dao/semi-app)
 - **后端代码 (Semi Backend)**：[https://github.com/nantang-dao/semi-backend](https://github.com/nantang-dao/semi-backend)
### 社区助手
 - **代码 (Bai)**：[[https://github.com/nantang-dao/Bai](https://github.com/nantang-dao/Bai)

开源项目代码使用 MIT License，向仓库提交代码即表示您认可以 MIT License 开源此代码。

## 三、角色与职责
### Maintainers（维护者）
 - **仓库管理**：负责管理仓库设置，包括 Label 管理、Project 看板维护、CI/CD 配置等。
 - **PR 审核与合并**：对 Pull Request（PR）进行 Code Review，确保代码质量，批准后合并进主分支。
 - **规划制定**：在 GitHub Projects 中规划 Roadmap，创建 Milestone。
 - **社区管理**：处理社区内的争议，维护社区秩序。

### Contributors（贡献者）
 - **内容提交**：提交 Issue 报告 Bug 或建议，提交 PR 贡献代码或文档。
 - **任务执行**：在 GitHub Project 中认领任务，并按时更新状态。
 - **规范遵守**：遵守代码规范与 Commit 规范。

### Community Members（社区成员）
 - **反馈建议**：提问、参与讨论，提供反馈与建议。
 - **测试推广**：协助测试新功能，传播项目理念。

**当前维护者 Maintainer**：jiang、云展、XHY

## 四、贡献类型
### 技术开发类
1. **数字钱包优化**

2. **社区助手迭代**

### 场景落地类
1. **需求调研**：根据社区真实应用情景，提交调研 Issue。
2. **案例沉淀**：记录落地案例，编写图文教程。

### 社区支持类
1. **新手帮扶**：解答 Issue 或 Discussions 中的新手问题。
2. **文档完善**：补充技术文档（如 ERC-4337 实现细节）或新手指引。

## 五、贡献流程 (GitHub Workflow)
为了保证多人协作不冲突，采用 **GitHub Project + Issue + PR** 的标准流。

### 第一步：认领任务 (Project & Issue)
1. 进入仓库的 **[Projects]** 页面，查看当前迭[线路图|roadmap]。**Todo**为待认领的任务。
    - 任务详情会标注任务类型（技术开发类、场景落地类、社区支持类）、难度等级（简单、中等、复杂）、验收标准以及激励方式。
    - 新手推荐筛选 Label 为 `good first issue` 的卡片。
2. **认领任务**：
    - 在你感兴趣的 Issue 下方评论：“**我想认领这个任务**”。
    - 等待 Maintainer 将该 Issue 分配给你（Assignees），并将卡片移动至 **In Progress** 栏。

### 第二步：开发与进度同步
1. **创建分支**：基于 `main` 分支创建你的开发分支。
    ```bash
    git checkout main
    git pull
    git checkout -b feat/task-system-optimization
    ```
2. **关联 Issue**：
    - 在开发过程中，如果是技术类任务，建议定期 Push 代码以防丢失。
    - 如果遇到困难，请直接在原 Issue 中评论寻求帮助，而不是私聊。

### 第三步：提交与验收 (Pull Request)
1. **提交 PR**：当功能开发完成或文档编写完毕后，提交 Pull Request。
2. **关联关闭 Issue**：在 PR 的描述（Description）中，务必包含关键字来自动关闭 Issue。
    - 例如：`Closes #123` 或 `Fixes #45`。
    - 这样当 PR 合并时，对应的 Issue 会自动移动到 **Done** 栏。
3. **Code Review**：
    - Maintainer 会对代码进行审查。
    - 请根据 Review 意见进行修改（直接在原分支 commit push 即可，PR 会自动更新）。
4. **合并与激励**：
    - PR 合并后，视为任务完成。
    - 凭合并记录在“社区助手”中领取相应的积分奖励。

## 六、GitHub Project 与 Issue 规范
### 1. Issue 提交规范
请使用提供的 **Issue Template**，或遵循以下格式：
- **标题**：清晰简练，如 `[Bug] 转账页面的地址显示错误`。
- **描述**：
    - **背景**：在什么场景下出现的？
    - **复现步骤**：1. 点击... 2. 输入...
    - **预期结果 vs 实际结果**。
    - **截图/日志**：必要的报错截图或 Log。
- **Label (标签)**：尽量为你的 Issue 打上标签（如 `bug`, `enhancement`, `documentation`）。

### 2. Project 看板管理
请使用 GitHub Projects 看板来可视化进度：
- **Todo**：待办事项池，所有经过确认的需求都在这里。
- **In Progress**：已分配且正在开发中。**每人原则上同时只能进行 1 个任务**。
- **Review**：代码已提交 PR，等待审核。
- **Done**：代码已合并，或任务已完成。

## 七、代码风格规范
1. **通用规范**：保持代码的一致性和可读性，遵循 DRY (Don't Repeat Yourself) 原则。
2. **JavaScript/TypeScript**：
    - 必须通过项目的 ESLint 检查。
    - 变量/函数使用 `camelCase`（小驼峰），类名使用 `PascalCase`（大驼峰）。
    - 必须定义明确的 TypeScript Interface，避免使用 `any`。
3. **Commit Message 规范**：
    - 遵循 Conventional Commits 规范：`type(scope): description`
    - 示例：`feat(wallet): add qr code scanning logic`
    - 常用 Type：`feat`(新功能), `fix`(修补), `docs`(文档), `style`(格式), `refactor`(重构), `chore`(杂项).

## 八、数据库相关贡献
### 数据库管理
1. **所有权**：
   - 由南塘DAO数字身份应用注册的用户，数据由南塘DAO开源小组拥有，进行管理。
   - 未来其他社区使用数字身份，并且希望单独托管的，在有自托管能力的前提下，可以使用自建的数据库进行自托管，或者获得数据备份。
2. **环境**：Supabase (PostgreSQL v17+)。

### 数据库安全
1. 每周定期备份数据库SQL，并且妥善存储备份文件
2. 数据库账户妥善保存，只有maintainer可以进行访问
3. 数据库账户和密码严禁写在文件代码中
### 表结构原则
1. **主键**：必须包含主键，推荐使用 UUID 或 Timestamp ID（String 格式），以字符串格式存储。
2. **字段**：使用 `snake_case` 统一命名（如 `user_id`, `created_at`）。
3. **扩展性**：建议具备明确的数据类型与长度，过长的可以使用 TEXT 存储可结构化数据，结构化数据可以用JSONB格式。
4. **安全**：严禁将数据库 Secret 提交到 Git 仓库，请使用 `.env` 文件。

## 九、测试策略
1. **强制测试**：核心功能（如转账、积分计算）必须包含单元测试。
2. **工具栈**：
    - 前端/合约：Jest / Vitest / Hardhat Test
    - 后端：Jest / Mocha
3. **PR 要求**：提交 PR 时，CI（持续集成）流水线必须全部通过。如果是新功能，需在 PR 描述中附带本地测试通过的截图。

## 十、贡献激励
1. 
2. 

---
感谢您对“乡建数字身份”开源社区的支持！
