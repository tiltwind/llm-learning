# 微调

## 1. 预训练 vs 微调

- **大模型训练（Pre-training）**  
  - **目标**：通过海量通用数据（如网页、书籍）学习语言的底层模式和知识（语法、逻辑、常识）。  
  - **方法**：无监督或自监督学习（如预测被遮挡的词、生成下一句话）。  
  - **特点**：需要巨量计算资源（数千张GPU/TPU）、长时间训练（数周至数月）。  
  - **输出**：通用基础模型（如GPT-3、BERT）。

- **微调（Fine-tuning）**  
  - **目标**：在预训练模型基础上，用特定领域数据（如医学文献、法律合同）适配具体任务（分类、问答）。  
  - **方法**：监督学习（使用标注数据调整模型参数）。  
  - **特点**：资源消耗低（单卡或少量GPU）、训练时间短（几小时至几天）。  
  - **输出**：领域专用模型（如医疗问答机器人）。

| **维度**       | **大模型训练**               | **微调**                     |
|----------------|----------------------------|-----------------------------|
| **数据**       | 通用数据（TB级）           | 领域数据（GB级）           |
| **任务**       | 学习语言基础能力           | 适配具体任务（如分类、生成） |
| **参数更新**   | 所有参数从头训练           | 部分或全部参数小幅调整     |
| **资源需求**   | 千亿级算力（如超算集群）   | 百亿级算力（如单台服务器） |
| **典型模型**   | GPT-4、LLAMA、PaLM         | ChatGPT（基于GPT-3微调）   |


## 2. 微调数据格式

参考： https://www.xfyun.cn/doc/spark/%E6%95%B0%E6%8D%AE%E9%9B%86%E6%A0%BC%E5%BC%8F%E8%AF%B4%E6%98%8E.html



## 3. 开放数据集

- Registry of Open Data on AWS, https://registry.opendata.aws/
- AI Studio数据集, https://aistudio.baidu.com/aistudio/datasetoverview, 百度AI Studio的人工智能学习与实训社区，提供开放数据集。
- 天池数据集, https://tianchi.aliyun.com, 阿里对外开放数据分享平台
- Papers With Code数据集, https://paperswithcode.com/datasets, 机器学习数据集
- Kaggle, https://www.kaggle.com/datasets, 包含各种有趣的数据集，如拉面评级、篮球数据等
- Hugging Face, https://huggingface.co/datasets,  AI社区，提供各种数据集
- CLUE 数据集, https://www.cluebenchmarks.com/dataSet_search.html, 中文数据集搜索引擎
- UCI 机器学习库, https://archive-beta.ics.uci.edu/
- Datasets for Data Science, Machine Learning, AI & Analytics, https://www.kdnuggets.com/datasets/index.html
- DataCastle数据科学学习社区, https://www.datacastle.cn/dataset_list.html
