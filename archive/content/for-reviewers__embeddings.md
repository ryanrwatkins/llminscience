As a starting place, here are initial recommendations of questions to be asked when reviewing research in which an LLM was used as part of their scientific research workflow.

- Were [embedding(s)](https://python.langchain.com/en/latest/modules/models/text_embedding.html?highlight=embedding) (i.e., [RA](https://aws.amazon.com/what-is/retrieval-augmented-generation/)[G](https://aws.amazon.com/what-is/retrieval-augmented-generation/)) used in the research?
- Is the tool used to create the [embedding](https://python.langchain.com/en/latest/modules/models/text_embedding.html?highlight=embedding) model provided and described?
- Were multiple [embeddings](https://python.langchain.com/en/latest/modules/models/text_embedding.html?highlight=embedding) created, tested, or used (i.e., chained)?
- Is the size of [chunks](https://python.langchain.com/en/latest/modules/indexes/text_splitters.html?highlight=chunks#text-splitters) used in preparing the data provided?
- Were different sizes of [chunks](https://python.langchain.com/en/latest/modules/indexes/text_splitters.html?highlight=chunks#text-splitters) tested for influence on LLM performance?
- Is the size of overlap permitted when creating [chunks](https://python.langchain.com/en/latest/modules/indexes/text_splitters.html?highlight=chunks#text-splitters) provided?
- Is the tool used for similarity matching (i.e., [vector database](https://python.langchain.com/en/latest/modules/indexes/vectorstores.html)) provided and described (e.g., FAISS)?
- Is the code available?

\* [Fine Tuning vs. Embeddin](https://www.linkedin.com/pulse/prompt-engineering-art-nudging-conversations-llm-fetahu-haxhiaj-msc/)[g](https://www.linkedin.com/pulse/prompt-engineering-art-nudging-conversations-llm-fetahu-haxhiaj-msc/)

Recommend Additions/Subtractions/Edits
Citable Article on LLM Norms and Review Criteria
