# 搭建教程

## OpenAI API使用指南
1. 注册OpenAI账号并获取API Key
2. 安装官方Python SDK：`pip install openai`
3. 示例代码：
```python
import openai

openai.api_key = 'your-api-key'
response = openai.Completion.create(
  model="text-davinci-003",
  prompt="Hello world"
)
print(response.choices[0].text)
```
- [官方快速入门](https://platform.openai.com/docs/quickstart)

## Anthropic API使用指南
1. 注册Anthropic账号并获取API Key
2. 安装官方Python SDK：`pip install anthropic`
3. 示例代码：
```python
import anthropic

client = anthropic.Client(api_key='your-api-key')
response = client.completion(
  prompt="Hello world",
  model="claude-v1"
)
print(response.completion)
```
- [官方文档](https://docs.anthropic.com/claude/docs/getting-started-with-the-api)

## DeepSeek API使用指南
1. 注册DeepSeek账号并获取API Key
2. 安装官方Python SDK：`pip install deepseek`
3. 示例代码：
```python
import deepseek

client = deepseek.Client(api_key='your-api-key')
response = client.generate(
  prompt="Hello world",
  model="deepseek-chat"
)
print(response.text)
```
- [官方文档](https://platform.deepseek.com/docs)

## 火山云API使用指南
1. 注册火山云账号并获取API Key
2. 安装官方Python SDK：`pip install volcengine`
3. 示例代码：
```python
from volcengine.llm import LLMClient

client = LLMClient(api_key='your-api-key')
response = client.generate(
  prompt="Hello world",
  model="volc-chat"
)
print(response.text)
```
- [官方文档](https://www.volcengine.com/docs/6561/102338)

## 硅基流动API使用指南
1. 注册硅基流动账号并获取API Key
2. 安装官方Python SDK：`pip install siliconflow`
3. 示例代码：
```python
from siliconflow import Client

client = Client(api_key='your-api-key')
response = client.generate(
  prompt="Hello world",
  model="sf-chat"
)
print(response.text)
```
- [官方文档](https://docs.siliconflow.com)

## 英伟达API使用指南
1. 注册英伟达开发者账号并获取API Key
2. 安装官方Python SDK：`pip install nvidia-api`
3. 示例代码：
```python
from nvidia import Client

client = Client(api_key='your-api-key')
response = client.generate(
  prompt="Hello world",
  model="nvidia-chat"
)
print(response.text)
```
- [官方文档](https://developer.nvidia.com/nvidia-api)