# 项目名（建议：EduMind / 研途问答 / SmartTutor，阶段 3 时定）

> 基于大模型 + Agentic RAG + LoRA 微调的领域智能问答系统

（此文件是未来项目仓库 README 的模板，项目启动后复制到 project/ 子目录使用）

## ✨ 项目亮点

- 🔍 **Agentic RAG**：基于 LangGraph 的"检索→反思→查询改写"循环，答不上不硬编
- 📊 **量化评估**：Ragas 指标（faithfulness / answer relevancy）+ 自建评测集，所有优化有数据支撑
- 🛠 **LoRA 微调**：LLaMA-Factory 微调 Qwen 小模型，领域问答效果对比提升 X%
- 📦 **工程化**：FastAPI + Docker Compose 一键部署，前端界面可交互

## 🏗️ 系统架构

（阶段 3 完成后补架构图：draw.io / processon 画）

```
文档 → 解析 → 分块 → BGE向量化 → 向量库
                                    ↓
用户问题 → 意图路由 → 查询改写 → 混合检索(BM25+向量) → 重排 → [反思: 相关?] → 生成(带引用)
```

## 🚀 快速开始

```bash
# 阶段 3 后填充
git clone https://github.com/<你的用户名>/<项目名>.git
cd <项目名>
docker compose up -d
# 打开 http://localhost:7860
```

## 📈 评估结果

（阶段 4 后填充对比表格）

| 配置 | Faithfulness | Answer Relevancy | 检索召回@5 |
|------|-------------|------------------|-----------|
| 基础 RAG | - | - | - |
| + 混合检索 + 重排 | - | - | - |
| + Agentic 反思 | - | - | - |
| + LoRA 微调 | - | - | - |

## 📄 License

MIT
