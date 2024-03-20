# HateCOT
Data repository for the paper "HateCOT: An Explanation-Enhanced Dataset for Generalizable Offensive Speech Detection via Large Language Models"
Link: https://arxiv.org/abs/2403.11456

**Abstract**:\
The ubiquitousness of social media has led to the need for reliable and efficient detection of offensive content to limit harmful effects. This has led to a proliferation of datasets and models related to detecting offensive content. While sophisticated models have attained strong performance on individual datasets, these models often do not generalize due to differences between how “offensive content” is conceptualized, and the resulting differences in how these datasets are labeled. In this paper, we introduce HateCOT, a dataset of 52,000 samples drawn from diverse existing sources with explanations generated by GPT-3.5-Turbo and human-curated. We show that pre-training models for the detection of offensive content on HateCOT significantly boots open-sourced Language Models on three benchmark datasets in both zero and few-shot settings, despite differences in domain and task. We further find that HateCOT enables effective K-shot finetuning in the low-resource settings.

**Description**:\
This dataset is curated from 8 openly available publications on offensive speech. 
Explanations to justify the post's corresponding labels are generated by GPT-3.5-Turbo. 
For detailed description of the curation process, please refer to the paper.

Pre-trained models (LLAMA 7B, LLAMA 13B) using this dataset will be uploaded to the HuggingFace hub.\

Data is stored in the file *hatecot_final_D3.csv*. \
*id*: native identififer of post from the original dataset \
*explanation*: explanations guided by human annotatations \
*domain*: 1 of the 8 original datasets the post is drawn from  \
*label*: the designated gold label of the post in the original work \
*post*: the anonymized content of the post \
*target*: the group(s) or individual(s) that the post's sentiment is directed towards \
*uid*: combination of id and domain, uniquely identify a row in this dataset 
