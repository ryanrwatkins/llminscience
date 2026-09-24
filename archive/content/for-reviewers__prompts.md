As a starting place, here are initial recommendations of questions to be asked when reviewing research in which an LLM was used as part of their scientific research workflow.

- Was an initial context or ‘seed’ used, and if so is it available?
- Was the [prompt](https://python.langchain.com/en/latest/modules/prompts.html) history empty when initial prompts were queried?
- Were multiple prompts created, tested, or used (i.e., [prompt engineering](https://help.openai.com/en/articles/6654000-best-practices-for-prompt-engineering-with-openai-api))?
- Was a data file(s) uploaded, and is a exact copy of that file available?
- Is the complete history of the prompting available?
- Are the dates/times of the prompts included with the history?
- Were [completion parameters](https://platform.openai.com/docs/api-reference/chat/create#chat/create-model) (e.g., temperature, presence penalty, frequency penalty, max tokens, logit bias) used and are those provided? [typically available through API only]
- Did completion parameters vary among prompts, and if so are those provided for each prompt?
- Were multiple combinations of [completion parameters](https://platform.openai.com/docs/api-reference/chat/create#chat/create-model) tested?
- Were quality review checks performed on LLM-generated results?
- Did the researcher(s) validate the LLM-generated results through experimentation or simulation?
- Is the code available?

Recommend Additions/Subtractions/Edits
Citable Article on LLM Norms and Review Criteria
