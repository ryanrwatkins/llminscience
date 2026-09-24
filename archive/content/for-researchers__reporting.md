Use the checklists below (depending on your use case) to verify that you are reporting the minimal required information for the transparent and reproducible use of LLMs (or genAI) in your research publications and report.

Recommend Additions/Subtractions/Edits

**Used LLM (or genAI) *Without* Parameter Adjustments**

- Provide name(s) and version(s) of the LLM (genAI) model(s) used.
  - If multiple models were tested during the research, include these along with a description of their application.
  - If model version is not available, include dates when used.
- Describe any custom instructions (e.g., “You are …”).
- Provide complete list of prompts tested and/or utilized (often as supplemental materials).
  - Describe prompting techniques tested and/or utilized (e.g., Chain of Thoughts, Tree of Thoughts, Program of Thoughts, etc.).
  - Describe how outputs were evaluated.

**Used LLM (or genAI) *With* Parameter Adjustments**

- Provide name(s) and version(s) of the LLM (genAI) model(s) used.
  - If multiple models were tested during the research, include these along with a description of their application.
- List the [completion parameter](https://platform.openai.com/docs/api-reference/chat/create#chat/create-model)[s](https://platform.openai.com/docs/api-reference/chat/create#chat/create-model) (e.g., temperature, presence penalty, frequency penalty, max tokens, logit bias).
- Describe any custom instructions (e.g., “You are …”).
- Provide a complete list of prompts tested and/or utilized (supplemental materials).
  - Describe prompting techniques tested and/or utilized (e.g., Chain of Thoughts, Tree of Thoughts, Program of Thoughts, etc.).
  - Describe how outputs were evaluated.

**Used Retrieval Augmented Generation (RAG)**

- Provide name(s) and version(s) of the LLM (genAI) model(s) used.
  - If multiple models were tested during the research, they should be included along with a description of their application).
- List the [completion parameter](https://platform.openai.com/docs/api-reference/chat/create#chat/create-model)[s](https://platform.openai.com/docs/api-reference/chat/create#chat/create-model) (e.g., temperature, presence penalty, frequency penalty, max tokens, logit bias).
- Describe how [embeddings](https://python.langchain.com/en/latest/modules/models/text_embedding.html?highlight=embedding) were created.
- Provide the size of [chunks](https://python.langchain.com/en/latest/modules/indexes/text_splitters.html?highlight=chunks#text-splitters) used in creating embeddings
- Provide the size of overlap permitted when creating [chunks](https://python.langchain.com/en/latest/modules/indexes/text_splitters.html?highlight=chunks#text-splitters)
- Provide and describe the tool(s) (e.g., FAISS) used for similarity matching (i.e., [vector database](https://python.langchain.com/en/latest/modules/indexes/vectorstores.html))
- Describe the retrieval tools/techniques will be used (e.g., [compression](https://python.langchain.com/docs/how_to/contextual_compression/), [context](https://www.anthropic.com/news/contextual-retrieval), [rerank](https://galileo.ai/blog/mastering-rag-how-to-select-a-reranking-model))
  - If external service(s) were used for reranking, list those.
- Describe any custom instructions (e.g., “You are …”).
- Provide a complete list of prompts tested and/or utilized (supplemental materials).
  - Describe prompting techniques tested and/or utilized (e.g., Chain of Thoughts, Tree of Thoughts, Program of Thoughts, etc.).
  - Describe how outputs were evaluated.

**Used** **Parameter-Efficient Fine-Tuning (PEFT) with LoRA or QLoRA** ***(or Similar**)*

- Provide name(s) and version(s) of the LLM (genAI) model(s) used.
  - If multiple models were tested during the research, include these along with a description of their application.
- List the [completion parameter](https://platform.openai.com/docs/api-reference/chat/create#chat/create-model)[s](https://platform.openai.com/docs/api-reference/chat/create#chat/create-model) (e.g., temperature, presence penalty, frequency penalty, max tokens, logit bias).
- If multiple parameter settings were tested during the research, describe these test.
- Describe the sources of data for PEFT fine-tuning. List separately for the development and evaluation of the updated model(s).
  - Describe the use of source(s) of data
  - Describe the use of existing data or collecting new data (if existing data were used, what was rationale)
  - Describe the use of synthetic data, if applicable
  - Describe all data preparation (e.g.., cleaning, imputation, transformations, partitions)

- List the [metrics](https://huggingface.co/metrics) used for PEFT evaluation.
- If weights were quantized (e.g., QLoRA), provide descriptions of tools used and process.
- List the PEFT hyperparameters tested and/or utilized (e.g., r, target\_modules).
- If Retrieval Augmented Generation (RAG) was used with the fine-tuned model(s), see RAG checklist above as well.
- What packages (and versions) were used (e.g., ollama 0.5.7, unsloth 2025.1.6)
- Describe any custom instructions are described (e.g., “You are …”).
- Provide a complete list of prompts tested and/or utilized (supplemental materials).
  - Describe the prompting techniques tested and/or utilized (e.g., Chain of Thoughts, Tree of Thoughts, Program of Thoughts, etc.).
  - Describe how outputs were evaluated.

**Used Full-Parameter Fine-Tuning**

- Provide name(s) and version(s) of the LLM (genAI) model(s) used.
  - If multiple models were tested during the research, include these along with a description of their application.
- List the [completion parameter](https://platform.openai.com/docs/api-reference/chat/create#chat/create-model)[s](https://platform.openai.com/docs/api-reference/chat/create#chat/create-model) (e.g., temperature, presence penalty, frequency penalty, max tokens, logit bias).
- If multiple parameter settings were tested during the research, describe these test.
- Describe the sources of data for fine-tuning. List separately for the development and evaluation of the updated model(s).
  - Describe the use of source(s) of data
  - Describe the use of existing data or collecting new data (if existing data were used, what was rationale)
  - Describe the use of synthetic data, if applicable
  - Describe all data preparation (e.g.., cleaning, imputation, transformations, partitions)
- Describe the approach to fine tuning described (e.g., Supervised Fine-Tuning (SFT), Reinforcement Learning from Human Feedback (RLHF)
- List the tools used for full parameter fine tuning (e.g., torchtune).
- If Retrieval Augmented Generation (RAG) was used with the fine-tuned model(s), see RAG checklist above as well.
- Describe any custom instructions are described (e.g., “You are …”).
- Provide a complete list of prompts tested and/or utilized (supplemental materials).
  - Describe the prompting techniques tested and/or utilized (e.g., Chain of Thoughts, Tree of Thoughts, Program of Thoughts, etc.).
  - Describe how outputs were evaluated.

**Used Multi-Agent System(s)**

- Provide name(s) and version(s) of the LLM (genAI) model(s) used.
- Provide the name(s) and version(s) of agent controller (e.g., [AutoGen](https://microsoft.github.io/autogen/)) used.
  - Describe the conversation pattern selected for use by agents.
  - Describe mechanisms for managing and coordinating the agents of agents.
- Provide details on the parameter adjustments for each agent.
- If Retrieval Augmented Generation ([RAG](for-researchers.qmd#section-reporting)) was used for one or more agents, describe those processes as outlined above.
- If fine-tuning ([PEFT](for-researchers.qmd#section-reporting) and/or [Full](for-researchers.qmd#section-reporting)) was used for one or more agents, describe those processes as outlined above.
- List the [completion parameter](https://platform.openai.com/docs/api-reference/chat/create#chat/create-model)[s](https://platform.openai.com/docs/api-reference/chat/create#chat/create-model) (e.g., temperature, presence penalty, frequency penalty, max tokens, logit bias), including if they are different for individual agents.
- Describe any custom instructions (e.g., “You are …”).
- Provide a complete list of prompts tested and/or utilized (supplemental materials).
  - Describe prompting techniques tested and/or utilized (e.g., Chain of Thoughts, Tree of Thoughts, Program of Thoughts, etc.).
  - Describe how outputs were evaluated.

---

\* *How to cite*: Watkins, R. (2024, September 25). *LLM in Science Publication Checklists*. LLMs in Scientific Research Workflows. https://llminscience.com/for-researchers/reporting/

\*\* The checklists above are based in part on the [TRIPOD+AI](https://www.bmj.com/content/385/bmj-2023-078378) [checklist](https://www.bmj.com/content/bmj/suppl/2024/04/18/bmj-2023-078378.DC6/colg078378.wt1.pdf). Additional reporting standards can be found in the [EQUATOR database](http://www.equator-network.org/).
