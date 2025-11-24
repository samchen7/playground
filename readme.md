# API Playground

一个功能完整的 API 测试和调试工具，支持多种大语言模型。

## 🚀 快速开始

```bash
python3 -m http.server 8888
```

访问：`http://localhost:8888`

## 使用步骤

1. 输入 API Key
2. 选择模型
3. 输入提示词和/或聊天记录
4. 调整参数（可选）
5. 点击发送请求

## 功能特性

- 支持 80+ 大语言模型（GPT、Claude、DeepSeek、Gemini、Grok、Qwen 等）
- 双输入模式：提示词 + 聊天记录
- 参数设置：Temperature、Max Tokens、Top P 等
- Token 管理：实时显示和限制检查
- 模型验证：自动验证模型名称

## ⚠️ 注意事项

- 模型名称需严格匹配，仅支持列表中的模型
- 默认 API 端点：`https://marketplace.aisa.one/pg/chat/completions`
- API Key 仅存储在浏览器本地
