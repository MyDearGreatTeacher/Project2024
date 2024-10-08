# [OpenAI API基礎必修課--使用Python(GPT-3.5、GPT-4、GPT-4o、DALL·E、TTS、Whisper模型)](https://www.tenlong.com.tw/products/9786263248106?list_name=srh)

# https://github.com/8wingflying/GenAI20240518/tree/main
# !pip install openai
```python
import openai
from google.colab import userdata
OPENAI_API_KEY= userdata.get('GenAI20240912')
client = openai.OpenAI(api_key=OPENAI_API_KEY)
```
```python
response = client.chat.completions.create(
    model = 'gpt-3.5-turbo',
    messages = [
        {'role': 'user', 'content': 'OpenAI 你好!'}
    ]
)

print(response)

print(response.choices[0].message.content)
```
