# InternLM-LangChain
1.大模型开发范式
大模型的局限性

![捕获](https://github.com/hui1feng/InternLM-LangChain/assets/126125104/90901248-7398-46c3-a91e-2e7d3987e5d8)

仅仅包含训练时间点之前的数据，无法回答更新的知识，且训练成本很高。
回答问题只有广度没有深度。
非定制模型解决客户需求能力受限。

核心大模型开发范式

![image](https://github.com/hui1feng/InternLM-LangChain/assets/126125104/b84511ff-7dc5-481c-b09c-a4d09bf1e326)

RAG：检索、增强、生成
  方式：模型外挂知识库提高大模型知识备。
  局限：单次回答有限总结性回答表现不佳
Finetun: 微调
		特点：对回答风格模拟特别好，对算力要求高。

![image1](https://github.com/hui1feng/InternLM-LangChain/assets/126125104/d84d0682-2e60-40a4-ada3-803feb3dba5c)


2.LangChain简介

![image2](https://github.com/hui1feng/InternLM-LangChain/assets/126125104/5063cc84-29e2-4fd5-9525-c0004211d539)

![image3](https://github.com/hui1feng/InternLM-LangChain/assets/126125104/5a8ec0e8-eb47-4945-b288-0b283d21355d)

首先加载各类格式本地文档->统一转化纯文本->分割成Chunk->准换为词向量存到Chroma数据库->将用户输入转化为同纬度向量->进行相似度对比->将相关文本段嵌入prompt->大模型回答

3.构建向量知识库

![image4](https://github.com/hui1feng/InternLM-LangChain/assets/126125104/36426982-b08e-437c-842c-ead3e544e33c)


4.搭建知识库助手

![image5](https://github.com/hui1feng/InternLM-LangChain/assets/126125104/22e254ac-062a-4722-a018-65149e4a470c)

![image6](https://github.com/hui1feng/InternLM-LangChain/assets/126125104/c389fe1b-5f23-4f75-9a7f-16800be80ed8)


问答性能有局限

![image7](https://github.com/hui1feng/InternLM-LangChain/assets/126125104/fdbca6f4-a962-410d-af0e-da546ca86428)

5.Web Demo部署

![image8](https://github.com/hui1feng/InternLM-LangChain/assets/126125104/04ed3768-6238-4774-9e16-ef6d5be77e65)


6.动手实践

