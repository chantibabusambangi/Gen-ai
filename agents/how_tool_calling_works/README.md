llm was connected to external tools.
say arxiv(research paper based) , wikipedia, and taviley(current/live news)
how the flow based on the query the tool calling works
like query: recent hot topic on ai and what is machine leanrng?
#obviously the llm can make tool recent hot topic on AI with tavily and what is machine leanrng? with wikipedia right.
but how the tool calls were done!?
**LLM extracts intents from user query Decides which tools to call for which subquery Calls Taviley, Wikipedia, Gets structured/clean data back from tools Synthesizes final answer and returns to user**

The LLM decides which tools to call based on:
The query content (intent detection).
Available tool capabilities.
Predefined tool routing logic.

High level WorkFlow:
✅ During runtime:
User query: “Recent hot AI topics.”
LLM parses and sees the need for live data.
Checks available tools:
Tavily available ✅
Wikipedia available ✅
Arxiv available ✅
Chooses Tavily for live data and Arxiv for recent papers.
