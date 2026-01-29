# Original task brief

# explain choice

# evaluation criteria

# reason for approach

<priyanka.pathak@dell.com>

Task: Develop an Information retriver that can fetch the most relevant documents from a set of articles and response generator that can generate proper responses for customer queries based on the retrieved context.

Dataset: <https://www.kaggle.com/datasets/harshsinghal/aws-case-studies-and-blogs>

Requirements:

1) Determine the vector store you will be using for the given data. Incorporate metadata with indexed vectors.

2) Optionally, try fine-tuning the embedding model with the provided data and share comparisons if only open-source embedding models are used.

3) Supervised finetune an open-source Large Language Model (LLM) with the given data. Explain how you prepare the dataset. Also, Enhance the Search Relevance with ReRank.

4) Explain the metrics used for evaluating both speed and quality of the model.

5) Suppose you have to deploy the system in production that has 4x A100 GPUs to cater to 1000 users per day. Explain how you will optimize the model to achieve high speed (average response time 1-2 seconds per user), leverage multi-core processors and parallel computing to distribute tasks and accelerate inference

6) Submit the code either through a Jupyter Notebook or a standalone Python file.

7) Solution to be submitted within 72 hrs.

Code submission should adhere to the requirements mentioned above.

## Resources that can be helpful

<https://github.com/jonfairbanks/local-rag/blob/develop/docs/pipeline.md>

llama 3 on colab and fine tuning:
<https://youtu.be/U-0dDikQGsc>

Fine tuning quantized LLM:
<https://huggingface.co/learn/cookbook/en/fine_tuning_llm_to_generate_persian_product_catalogs_in_json_format#fine-tuning-llm-to-generate-persian-product-catalogs-in-json-format>

--------------------------------------------------------------------------------

## Useful Links for Dataset preparation & Metadata

- <https://www.reddit.com/r/LangChain/comments/15niet1/using_document_metadata_in/>
- <https://github.com/langchain-ai/rag-from-scratch>
- <https://bibek-poudel.medium.com/extract-metadata-using-langchain-gpt-4-and-retrieval-augmented-generation-rag-15ae9ddce236>
- <https://akash-mathur.medium.com/advanced-rag-optimizing-retrieval-with-additional-context-metadata-using-llamaindex-aeaa32d7aa2f> && <https://github.com/akashmathur-2212/LLMs-playground/blob/main/LlamaIndex-applications/Advanced-RAG/parent_child_document_retriever/parent_child_document_retriever_metadata_extraction.ipynb>
- <https://github.com/langchain-ai/langchain/discussions/10983#discussioncomment-7647999>

## Useful Links for Retrieval & ReRanking

- <https://python.langchain.com/v0.1/docs/modules/data_connection/retrievers/ensemble/>
- <https://python.langchain.com/v0.2/docs/integrations/retrievers/cohere-reranker/>

## Useful Links for Fine Tuning

- <https://github.com/aws-samples/fine-tuning-llm-with-domain-knowledge/blob/main/src/fine_tuning.ipynb>
- <https://www.philschmid.de/fine-tune-flan-t5-peft>
- <https://pytorch.org/blog/finetune-llms/> --> <https://colab.research.google.com/drive/1vIjBtePIZwUaHWfjfNHzBjwuXOyU_ugD?usp=sharing>
- <https://huggingface.co/learn/cookbook/rag_zephyr_langchain> && <https://www.datacamp.com/tutorial/zephyr-7b-tutorial>
- <https://github.com/unslothai/unsloth>
- Model choice: <https://huggingface.co/spaces/Intel/low_bit_open_llm_leaderboard>

## Useful Links for Evaluation

- <https://docs.smith.langchain.com/concepts/evaluation>
- <https://docs.smith.langchain.com/tutorials/Developers/rag#evaluator>
- <https://www.perplexity.ai/search/please-act-as-llm-expert-and-h-ZTeiN6pjSZWfo66ulTnzHA>

## Useful Links for embedding models

- <https://www.sbert.net/examples/applications/retrieve_rerank/README.html?highlight=information%20retrieval>
- <https://www.sbert.net/docs/sentence_transformer/training_overview.html>

--------------------------------------------------------------------------------

### Comparison on Fine Tuning techniques

![LoRA v/s QLoRA](image.png)

### VRAM Requirement

<https://www.reddit.com/r/LocalLLaMA/comments/18o5u0k/helpful_vram_requirement_table_for_qlora_lora_and/>
![VRAM Requirement](image-1.png)

### Test App 
![gradio_base_llm](image-2.png)