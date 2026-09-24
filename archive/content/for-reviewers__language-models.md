As a starting place, here are initial recommendations of questions to be asked when reviewing research in which an LLM was used as part of their scientific research workflow.

- Which [language model](https://python.langchain.com/en/latest/modules/models/llms/integrations.html) was [fine tuned](https://bdtechtalks.com/2023/07/10/llm-fine-tuning/#:~:text=In%20such%20situations%2C%20one%20of,that%20should%20come%20to%20mind.) (e.g., OpenAI’s GPT-3.5 model)?
- Which (if any) packages were used (e.g., [DSPy](https://github.com/stanfordnlp/dspy), [RAG](https://github.com/explodinggradients/ragas)[AS](https://github.com/explodinggradients/ragas), etc.)?
- Were multiple [language models](https://python.langchain.com/en/latest/modules/models/llms/integrations.html) tested for performance before selecting?
- What tool(s) were used for fine tuning to model (e.g., [LoR](https://bdtechtalks.com/2023/05/22/what-is-lora/)[A](https://bdtechtalks.com/2023/05/22/what-is-lora/), [PEFT](https://www.mercity.ai/blog-post/fine-tuning-llms-using-peft-and-lora#what-is-peft), [OpenAI tool](https://platform.openai.com/docs/guides/fine-tuning)[s](https://platform.openai.com/docs/guides/fine-tuning))?
- Which data were used for [fine tunin](https://platform.openai.com/docs/guides/fine-tuning)[g](https://platform.openai.com/docs/guides/fine-tuning)?
- Was splitting (training/testing) used, and if so what proportions (e.g., 80/20)?
- Which (if any) [evaluation libraries](https://github.com/openai/evals) were used to assess the fine tuned model?
- Did the researcher(s) evaluate the LLM’s performance against other benchmarks or standards?
- Is the code available?

\* *Note that at this time there are no standards for setting completion parameters (such as temperature). As standards come available we will post updates.*

\*\* [Fine Tuning vs. Embeddin](https://www.linkedin.com/pulse/prompt-engineering-art-nudging-conversations-llm-fetahu-haxhiaj-msc/)[g](https://www.linkedin.com/pulse/prompt-engineering-art-nudging-conversations-llm-fetahu-haxhiaj-msc/)

Recommend Additions/Subtractions/Edits
Citable Article on LLM Norms and Review Criteria
