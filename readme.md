# API Playground

一个功能完整的 API 测试和调试工具，支持多种大语言模型。

## ✨ 功能特性

- **API 配置**：API Key 输入、API 端点配置（默认：`https://marketplace.aisa.one/pg/chat/completions`）
- **模型选择**：支持 80+ 大语言模型，严格遵守模型名称规范
- **双输入模式**：
  - 提示词（指令方向）
  - 聊天记录（原材料）
  - 两者可同时使用
- **参数设置**：Temperature、Max Tokens、Top P、Frequency/Presence Penalty、Token 限制
- **Token 管理**：实时显示输入/输出 Token，自动检查限制
- **模型验证**：自动验证模型名称，确保使用支持的模型
- **响应显示**：深色代码风格，支持多种响应格式

## 🚀 快速开始

```bash
# 启动服务
python3 -m http.server 8888
```

访问：`http://localhost:8888`

### 使用步骤

1. 输入 API Key（API 端点已默认配置）
2. 从下拉菜单选择模型
3. 输入提示词和/或聊天记录
4. 调整参数（可选）
5. 点击发送请求

## 📋 支持的模型

系统严格遵守以下模型列表，仅支持以下模型：

### GPT 系列
- gpt-4.1, gpt-4o, gpt-4o-mini, gpt-5, gpt-5-mini

### Claude 系列
- claude-3-5-haiku-20241022
- claude-3-7-sonnet-20250219, claude-3-7-sonnet-20250219-thinking
- claude-opus-4-1-20250805, claude-opus-4-1-20250805-thinking
- claude-opus-4-20250514, claude-opus-4-20250514-thinking
- claude-sonnet-4-20250514, claude-sonnet-4-20250514-thinking
- claude-sonnet-4-5-20250929

### DeepSeek 系列
- deepseek-r1, deepseek-v3, deepseek-v3-0324, deepseek-v3.1

### Gemini 系列
- gemini-2.5-flash, gemini-2.5-flash-lite, gemini-2.5-pro

### Grok 系列
- grok-3, grok-3-mini-beta, grok-4, grok-4-0709

### Qwen 系列
- qwen-max, qwen-max-latest, qwen-mt-plus, qwen-mt-turbo
- qwen-plus, qwen-plus-2025-04-28, qwen-plus-latest
- qwen-turbo, qwen-turbo-1101, qwen-turbo-2025-04-28, qwen-turbo-latest
- qwen-vl-max, qwen-vl-plus
- qwen2-vl-72b-instruct, qwen2-vl-7b-instruct
- qwen2.5-14b-instruct-1m, qwen2.5-32b-instruct, qwen2.5-3b-instruct
- qwen2.5-72b-instruct, qwen2.5-7b-instruct-1m
- qwen2.5-vl-72b-instruct, qwen2.5-vl-7b-instruct
- qwen3-0.6b, qwen3-1.7b, qwen3-14b, qwen3-235b-a22b
- qwen3-235b-a22b-instruct-2507, qwen3-30b-a3b, qwen3-32b
- qwen3-4b, qwen3-8b
- qwen3-coder-480b-a35b-instruct, qwen3-coder-plus, qwen3-coder-plus-2025-07-22
- qwen3-max, qwen3-max-preview, qwen3-vl-235b-a22b-instruct

### 其他
- sora-2, sora-2-pro
- text-embedding-3-large, text-embedding-3-small

## ⚠️ 注意事项

- **模型名称严格匹配**：系统会自动验证模型名称，仅允许使用上述列表中的模型
- **API 端点**：默认使用 `https://marketplace.aisa.one/pg/chat/completions`，可根据需要修改
- **API Key 安全**：API Key 仅存储在浏览器本地，不会发送到任何第三方服务器
