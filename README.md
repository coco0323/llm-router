🚀 LLM Router

Reduce LLM API cost by automatically routing between DeepSeek, Qwen, and Doubao.

⸻

💡 What is this?

LLM Router is a drop-in OpenAI-compatible API that automatically selects the cheapest and best-performing model for your request.

Instead of manually choosing models, just use:
model="auto"

⸻

 Features

* 🔀 Multi-model routing ( glm / kimi / Qwen / Doubao)
* 💰 Cost optimization (save up to 80%)
* ⚡ OpenAI-compatible API (zero migration cost)
* 🔁 Automatic fallback on failure
* 🧠 Smart model selection based on task type

⸻

* 🚀 Quick Start
* from openai import OpenAI

client = OpenAI(
  base_url="https://your-api.com/v1",
  api_key="your-key"
)

res = client.chat.completions.create(
  model="auto",
  messages=[
    {"role": "user", "content": "write a marketing plan"}
  ]
)
print(res)

⸻

💰 Why use LLM Router?

Using a single model is expensive and inefficient.

LLM Router automatically routes:

* Simple tasks → Doubao (cheapest)
* Balanced tasks → Qwen
* Complex reasoning → kimi/glm

⸻

🔥 Result

* Up to 80% cost reduction
* No code changes required
* Plug-and-play API

📦 Status

🚧 Active development



