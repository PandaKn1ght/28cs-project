# 阶段 2：大模型基础 + Prompt 工程（第 7-10 周，约 40h）

**目标**：理解大模型"从训练到使用"的全流程，本地和云端模型都能跑起来，掌握 Prompt 工程的核心套路。

## 任务清单

### 第 7 周：大模型原理深入
- [ ] 预训练：数据规模、scaling law 概念
- [ ] SFT：指令微调数据长什么样（instruction / input / output）
- [ ] RLHF：奖励模型 + PPO 的直觉；DPO 是什么（概念）
- [ ] Hugging Face：transformers 加载 tokenizer 和模型，跑一次 generate()

### 第 8 周：本地部署 + API
- [ ] 安装 Ollama，跑通 `ollama run qwen2.5:3b`（先小后大）
- [ ] 对比 3B 和 7B 模型的回答质量和速度（记录到笔记）
- [ ] 申请 DeepSeek / 智谱 GLM API key，用 Python SDK 完成对话调用
- [ ] 理解 API 参数：temperature / top_p / max_tokens / system prompt

### 第 9 周：Prompt 工程
- [ ] DataWhale llm-cookbook 前几门课（Prompt 开发原则、迭代、摘要/推理/转换/扩展）
- [ ] Few-shot：什么时候有用？示例怎么选？
- [ ] 思维链（CoT）：什么任务上提升明显？
- [ ] 结构化输出：让模型稳定输出 JSON（Pydantic 校验 + 解析失败重试）
- [ ] 系统提示词设计：角色设定、约束、输出格式

### 第 10 周：小项目——命令行聊天机器人
- [ ] 多轮对话历史管理（滑动窗口/摘要压缩二选一）
- [ ] 流式输出（打印逐 token）
- [ ] system prompt 可配置；支持切换本地 Ollama / 云端 API
- [ ] 代码推 GitHub，写 Prompt 实验笔记博客 1 篇

## 自测题

1. RLHF 的完整流程？为什么需要奖励模型？
2. temperature=0 和 temperature=1.5 分别会发生什么？
3. 大模型怎么做到输出合法 JSON 的？失败了怎么办？
4. 上下文窗口（context window）是什么？超长了怎么办？

## 笔记区

