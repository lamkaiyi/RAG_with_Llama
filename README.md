# RAG_with_Llama
A simple demonstration of Retrieval Augmented Generation (RAG) pipeline constructed and evaluated using Llama2 models.

The pipelines were constructed using both LlamaIndex and LangChain.


# Motivations 

Evaluation of RAG pipelines require an external LLM. Most evaluation tools use OpenAI models under the hood in providing evaluation metrics. While powerful and effective, they are not free to use and can incur significant costs over time.

These test examples aim to construct basic RAG pipelines, and evaluate them without the use of OpenAI models.

The examples aim to explore how different (and free to use) RAG evaluation frameworks can be integrated into a basic RAG pipeline, to offer insights into the performance of said pipeline. Such insights can then be used for further finetuning.

# Constraints and Limitations

As this code is demonstrative in nature, it should run out-of-the-box without the need for excessive modifications. 

Further to making the code as accessible as possible, we aim to be able to run all code within a Google Colabatory environment using free tier GPUs. Inevitably, this will introduce certain constraints, namely:

- The choice of LLM would have to be one with a lower number of parameters, to avoid consuming excessive disk space.

  
- The same LLM will be used to generate responses, and evaluate the responses. In practice, a different and "better" LLM should always be used for evaluation.

# Requirements

Additional resources required to run the code are listed below. As of Jan 2024, these are open source and free for access:

- HuggingFace account and API key (https://huggingface.co/docs/transformers.js/guides/private)
- Authorization to use Llama2 models (https://ai.meta.com/resources/models-and-libraries/llama-downloads/)

**Note**: ensure that you request authorization with the same email address as your HuggingFace account. After which, request access here (https://huggingface.co/meta-llama/Llama-2-13b) 

