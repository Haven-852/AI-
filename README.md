# AI应用开发师学习案例
用于记录在github当中的AI应用开发师所需要的能力以及优秀学习案例

## Function Calling
https://github.com/mshojaei77/simple_function_calling

description：Function calling allows LLMs to interact with external tools or APIs by generating structured JSON that describes function calls. This capability helps transform natural language queries into actionable API calls. For example, a model could determine that a user wants to know the current weather and generate JSON to call a weather API.

## microGPT
核心思想其实是：把 GPT 的本质压缩成最小可理解版本，训练流程只有几步：

```
text -> tokenizer -> token ids  
        ↓  
embedding  
        ↓  
self-attention  
        ↓  
MLP  
        ↓  
预测下一个 token  
        ↓  
loss  
        ↓  
backprop  
        ↓  
Adam 更新参数
```
这个 200 行代码基本完整复现：

- Self-Attention

- Transformer block

- RMSNorm

- KV cache

- Temperature sampling

链接：项目介绍：https://karpathy.github.io/2026/02/12/microgpt/?utm_source=chatgpt.com 
项目地址：https://gist.github.com/karpathy/8627fe009c40f57531cb18360106ce95 
