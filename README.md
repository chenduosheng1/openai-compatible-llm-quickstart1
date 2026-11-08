# 便宜的 OpenAI 兼容 API（DeepSeek 闲时低至 2.5 折）

不想被各家大模型厂商高价按量收割？这是一个 **OpenAI 兼容** 的 API 中转/聚合服务，代码一行不改，把 `base_url` 换成下面地址就能用。

## 为什么用 5pcloud.top

- **闲时 DeepSeek 低至 2.5 折**：深夜/闲时用 DeepSeek 跑批、跑 Agent 成本直接砍到脚踝。
- **注册送 1000 万 token**：新用户上来就能白嫖跑通你的应用。
- **支付宝 10 元起充**：不用办双币信用卡，国内钱包直接充。
- **OpenAI 兼容**：OpenAI SDK、LangChain、NextChat、LobeChat、SillyTavern、OpenWebUI 全都直接接。

## 30 秒接入

```python
from openai import OpenAI

client = OpenAI(
    base_url="https://5pcloud.top/v1",
    api_key="你的密钥",  # 注册后在控制台获取
)

resp = client.chat.completions.create(
    model="deepseek-chat",
    messages=[{"role": "user", "content": "你好"}],
)
print(resp.choices[0].message.content)
```

## 支持的客户端

| 客户端 | 配置 |
| --- | --- |
| NextChat | API Base: `https://5pcloud.top` |
| LobeChat | 自定义接口: `https://5pcloud.top` |
| SillyTavern | API 类型 OpenAI，地址 `https://5pcloud.top` |
| OpenWebUI | OPENAI_API_BASE_URL=`https://5pcloud.top/v1` |

## 立即注册

👉 [注册领取 1000 万 token，闲时 DeepSeek 低至 2.5 折](https://5pcloud.top/?src=github_readme)

> 本站为第三方聚合服务，与官方模型厂商无隶属关系。
