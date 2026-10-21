# PlanRecord RAG 客服助手

独立于 PlanRecord 网页项目的 Dify 应用备份。备份日期：2026-10-21（Asia/Shanghai）。

## 备份内容

- `dify/app.yml`：从已登录的 Dify 工作室实际导出的应用 DSL，版本 0.7.0。
- `knowledge/`：从 Dify 文档列表逐一下载的全部 3 份原始文件。
- `RESTORE.md`：已核实的模型、检索设置与恢复步骤。
- `SHA256SUMS.json`：上述导出文件的 SHA-256 校验值。

应用为 RAG 聊天助手（mode: chat，agent_mode.enabled: false），不是自主工具调用 Agent。
模型为 qwen3.8-flash，应用级重排为 qwen3-rerank，Top K 为 4。
在线入口：https://udify.app/chat/gs3XbpNKWUMeZiBs

本仓库只保存 RAG 助手资料，不包含网站源代码，也不触发网站部署。
未包含模型服务密钥、聊天日志、云端向量索引或手动修改后的分段快照。恢复需重新配置凭据、创建知识库并重新索引；本次未在新工作区执行恢复测试。
