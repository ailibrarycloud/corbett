# Corbett by AI Library
Explore multi-model AI models and build AI applications without coding

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


## FAQs

### Can I collaborate with other people/teams on Corbett?
Yes you can. Once you upload your files in Corbett, it generates a knowledge ID. You can share this knowledge ID with other users (or your team) and you can collaborate with them.

### Can I give html links as a knowledge source in Corbett?
Yes you can. Corbett will extract text from the webpage and use it as a knowledge source, but we recommend that you save the page first on your local resource and then upload it on Corbett.

### How much data do I need to upload in order for the LLM to answer my queries? 
The quality of the answer is dependent on the quality of the knowledge base. Remember, the LLM cannot give an answer to a query which doesn’t have an answer in the knowledge base. It’s a matter of quality not quantity.

### What if Corbett is not able to answer my question or gives the wrong answer?
You can try changing the LLM that you are using, we provide a wide range of commercially available and open source models. If it still doesn’t work, then the LLMs may be having difficulty in processing the question. We recommend rephrasing the question in this case. If the answer is still not satisfactory there might be other problems, for instance, it may happen that the knowledge base doesn’t have an answer. In rare cases, the LLM might be hallucinating. 

### Can Corbett process diagrams in the knowledge base?
It depends on the complexity of the diagram and the particular LLM being used.
