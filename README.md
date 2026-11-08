# openai-compatible-llm-quickstart

一行 base_url，接好你的 OpenAI 兼容大模型 API。

## Ara API — 注册送 1000 万 DeepSeek token，闲时低至 2.5 折

兼容 OpenAI SDK，Cursor / Claude Code / LobeChat / n8n 改一处 `base_url` 即用。

- 注册即送 **1000 万 DeepSeek token**（免费试用）
- **闲时低至 2.5 折**（DeepSeek 系列）
- 支付宝 **10 元起充**，额度秒到账，不绑卡
- 5 分钟接入，先跑通再付费

### 快速开始

```bash
export OPENAI_API_KEY="你的Ara密钥"
export OPENAI_BASE_URL="https://5pcloud.top/v1"
```

```python
from openai import OpenAI
client = OpenAI(api_key="你的Ara密钥", base_url="https://5pcloud.top/v1")
resp = client.chat.completions.create(
    model="deepseek-chat",
    messages=[{"role": "user", "content": "你好"}],
)
print(resp.choices[0].message.content)
```

### 注册

免费注册领取 1000 万 token：https://5pcloud.top/register.html?src=github

### 文档

- 接入指南：https://5pcloud.top/quickstart.html?src=github
- 价格：https://5pcloud.top/models.html?src=github
- 博客教程：https://5pcloud.top/blog/

---

低成本 OpenAI 兼容 API · DeepSeek 闲时 2.5 折 · 注册送 1000 万 token
