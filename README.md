<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/subaru-ye/subaru-ye/main/assets/header-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/subaru-ye/subaru-ye/main/assets/header-light.svg">
  <img alt="Subaru Ye · 白桦 — Java / Go / AI 应用开发" src="https://raw.githubusercontent.com/subaru-ye/subaru-ye/main/assets/header-light.svg" width="100%">
</picture>

我是 **白桦（subaru-ye）**，华东交通大学软件工程本科在读，主攻 **Java 后端与 AI 应用工程化**，也使用 Go 构建 Agent 工具、参与开源开发工具的缺陷定位与修复。

## 开源贡献

已合并的代表修复：

| 项目 | 解决的问题 | 已合并 PR |
| :--- | :--- | :--- |
| **roborev** | 修复 Git hooks 自动维护修改工作区文件的问题，覆盖关联 worktree 场景，补充回归测试与文档。 | [#1178](https://github.com/kenn-io/roborev/pull/1178) |
| **roborev** | 改进历史审查提示，避免重复报告已修复问题或要求撤销修复，补充回归测试。 | [#1271](https://github.com/kenn-io/roborev/pull/1271) |

**OpenCodeReview · 缺陷定位与验证**：提供流式工具调用元数据丢失的复现，发现负索引处理缺陷，并在 Windows 上完成 race detector 验证。最终合并的 [#1393](https://github.com/alibaba/open-code-review/pull/1393) 明确致谢该复现工作；[定位与验证过程](https://github.com/alibaba/open-code-review/pull/1233#issuecomment-5690930354)。

<details>
<summary>其他贡献与讨论</summary>

- [OpenCodeReview #1539](https://github.com/alibaba/open-code-review/pull/1539)：为 Windows glob 路径误用提供警告，覆盖命令行参数与规则配置。
- [roborev #1332](https://github.com/kenn-io/roborev/pull/1332)：为审查提示补充项目声明的 Go 版本上下文。
- [pi #9361](https://github.com/earendil-works/pi/issues/9361#issuecomment-5676474857)：参与扩展工具丢失 shell 配置问题的定位、复现与方案讨论。

以上为其他贡献记录；当前状态以各链接中的 GitHub 记录为准。

</details>

## 代表项目

### [装机配置单 Agent](https://github.com/subaru-ye/pc-builder-agent)

面向预算与用途的对话式装机助手，支持需求确认、配置生成、增量改单和版本对比。

- **工程重点**：LLM 负责意图与解释，规则引擎负责兼容性与核算；交付前复验，保留报价日期与证据。
- **技术栈**：Go · A2A · PostgreSQL / pgvector · Redis · Next.js
- [架构、运行与评估文档](https://github.com/subaru-ye/pc-builder-agent/tree/main/docs)

### [白桦网站秒搭](https://github.com/subaru-ye/ye-ai-web-factory)

基于自然语言的 AI 网站生成平台，支持流式生成、代码下载与一键部署。

- **工程重点**：AI 生成链路、对话上下文管理、生成模式解耦与安全护轨。
- **技术栈**：Java · Spring Boot · LangChain4j · Redis · SSE
- [项目介绍](https://baihua.vercel.app/#projects) · [源码](https://github.com/subaru-ye/ye-ai-web-factory)

### [Brain Rush · AI 闯关学习](https://github.com/subaru-ye/brain-rush)

输入学习主题或材料，生成闯关题并获得即时讲解，完成后生成复盘报告，通过学习历史与错题本继续复训。

- **工程重点**：pgvector 混合 RAG 优先召回自维护题库与知识片段，结合 AI 补题；提供知识库管理、异步资料导入与检索评估。
- **技术栈**：Python · FastAPI · LangChain · PostgreSQL / pgvector · Redis / RQ · Taro / React / TypeScript
- [功能与本地启动说明](https://github.com/subaru-ye/brain-rush#readme) · [设计与 RAG 文档](https://github.com/subaru-ye/brain-rush/tree/main/docs)

### [Tonight 云图库](https://github.com/subaru-ye/ye-picture)

全栈图片管理系统，支持 AI 标注、团队空间、权限控制与实时协同编辑。

- **工程重点**：空间级 RBAC、WebSocket 协作、RabbitMQ 异步通知，以及原图 / 压缩图 / 缩略图分级存储。
- **技术栈**：Java · Spring Boot · MySQL · Redis · RabbitMQ · Vue / TypeScript
- [功能与本地启动说明](https://github.com/subaru-ye/ye-picture#readme)

另有 [算法复盘](https://algo-replay.vercel.app/)：基于间隔重复的算法学习工具，使用 React / Vite 构建；[源码](https://github.com/subaru-ye/algo-replay)。

## 技术方向

| 方向 | 项目中使用的技术 |
| :--- | :--- |
| 后端与数据 | Java / Go · Spring Boot · MySQL / PostgreSQL · Redis · RabbitMQ |
| AI 应用 | 工具调用 · Agent 工作流 · A2A · 规则校验 · 评估与回归验证 |
| 前端与交付 | Vue / React · TypeScript · Next.js · Docker · Git |

通过[个人作品集](https://baihua.vercel.app/)了解更多项目，或发送邮件至 [838184610@qq.com](mailto:838184610@qq.com)。
