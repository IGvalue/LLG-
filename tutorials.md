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