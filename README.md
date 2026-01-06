# 🚀 apifree-ai-resource  
免费、易用的AI API资源聚合平台 | [官网直达](https://www.apifree.ai/explore)


## 🌟 什么是 apifree.ai？
apifree 是一个**完全免费**的AI服务平台，提供各类AI能力的API接口（如大模型对话、图像生成、语音处理等），无需复杂配置，注册即可快速调用，适合开发者、学生、个人项目快速集成AI功能。


## 🛠️ 快速上手（5分钟接入）
以「调用对话API」为例：
1. 前往 [apifree官网](https://www.apifree.ai/explore) 注册账号，获取你的API Key
2. 调用示例（Python）：
```python
import requests

url = "https://api.apifree.ai/v1/chat/completions"
headers = {
    "Authorization": "Bearer 你的API_KEY",
    "Content-Type": "application/json"
}
data = {
    "model": "gpt-3.5-turbo",
    "messages": [{"role": "user", "content": "介绍一下你自己"}]
}

response = requests.post(url, headers=headers, json=data)
print(response.json()["choices"][0]["message"]["content"])
