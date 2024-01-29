# Corbett by AI Library
Explore AI models and create AI applications without coding

## Introduction

Generative AI can be used in various ways to derive insights from various knowledge sources (unstructured or structured databases). Corbett is a no-code platform that can import various types and formats of data to generate these insights. While several platforms exist for this, Corbett allows one to use diverse AI models available by providers like OpenAI, Cohere etc in one place and benchmark the results from these various
models.

Corbett is able to generate these insights from the data that the user provides by using cutting edge RAG (Retrieval Augmented Generation) techniques, which involve providing the data in the context window rather than using it to fine tune the LLM directly. Fine tuning is expensive and previous attempts at fine tuning the LLM were only partly successful. Our approach involves providing the knowledge base (both structured and unstructured databases) in the context window and re-prompting the model (RAG). This method has been shown to be more adept at capturing insights from the data. We also use prompt engineering techniques for optimising the model and returning the required output. These prompt engineering techniques include augmenting the unstructured data that is passed as vector embeddings to the context window to generate the desired output. In the case of structured data we make use of our no-code capabilities to convert the natural language query to an sql or python code, then we execute this code to give us the answer to the query. 

The user can also use news as a knowledge source or use our platform to summarise results from their favourite search engine. In the latest version you can also use Youtube videos as a knowledge source and generate insights using our cutting edge algorithms.

Besides this the user can add her/his own knowledge sources in formats that are listed below. She/he can query the available models which will be focussed on these knowledge sources to provide insights.

## Explore AI Models

The following table list of AI models we currently provide access

| Provider | Type | Models |
| -------- | ------- |------- |
| OpenAI  | text-to-text    | gpt-4-1106-preview, gpt-3.5-turbo    |
| OpenAI | text-to-image     | dall-e-3    |
| OpenAI    | text-to-speech    | tts-1, tts-1-hd    |
| Google  | text-to-text    | gemini, bison    |
| Meta | text-to-text     | llama-7b3    |
| Anthropic    | text-to-text    | claude-2.1    |
| Stability AI  | text-to-image    | stable-diffusion-xl-1024-v1-0    |
| Cohere | text-to-text     | commando    |
| AI21    | text-to-text    | j2-mid    |

## Build a Knowledge Base

To restrict LLMs to custom data, you can build a knowledge base by uploading data or connecting to a data source. 

### Supported Data Formats

.doc
.docx
.pdf
.pptx
.txt

### Integrations

| Name | Provider | Type |
| -------- | ------- | ------- |
| News  | Bing (Microsoft) | Real-time |
| Search  | Bing (Microsoft) | Real-time |
| YouTube  | YouTube (Google) | One-time |



