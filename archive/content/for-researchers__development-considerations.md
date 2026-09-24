As a starting place, here are initial recommendations of questions to be asked when considering the use of an LLM as part of your scientific research workflow.

- What protocols (guidelines) have been developed to ensure systematic use of LLMs?
- What [completion parameter](https://platform.openai.com/docs/api-reference/chat/create#chat/create-model)[s](https://platform.openai.com/docs/api-reference/chat/create#chat/create-model) (e.g., temperature, presence penalty, frequency penalty, max tokens, logit bias) will be used?
- Are pre-established decisions related to completion parameters readily available to those prompting the LLM?
- Will [embeddings](https://python.langchain.com/en/latest/modules/models/text_embedding.html?highlight=embedding) be utilized in the research?
- What size [chunks](https://python.langchain.com/en/latest/modules/indexes/text_splitters.html?highlight=chunks#text-splitters) will be used in creating embeddings?
- What size of overlap permitted when creating [chunks](https://python.langchain.com/en/latest/modules/indexes/text_splitters.html?highlight=chunks#text-splitters) provided?
- What tool(s) will be used for similarity matching (i.e., [vector database](https://python.langchain.com/en/latest/modules/indexes/vectorstores.html)) provided and described (e.g., FAISS)?
- Will embedding files be publicly available after the research is complete?
- Will [LLM agent(s)](https://python.langchain.com/en/latest/modules/agents.html) be used in the research?
- Will any code associated with the use of LLMs documented?
- Will the code be publicly available ?
- Will LLM responses be systematically checked for accuracy, bias, and other limitations?
- What data management systems will put in place to secure the data (inputs and outputs) of the LLMs?

Recommend Additions/Subtractions/Edits
