# Research Rabbit 🐰

A fully local web research and summarization agent that autonomously explores topics in depth through iterative research cycles.

## 🚀 Quickstart with LangGraph server, Ollama and Tavily

Pull a local LLM that you want to use from [Ollama](https://ollama.com/search):
```
ollama pull llama3.1
```

Install the langgraph CLI:
```
pip install -U "langgraph-cli[inmem]"
```

Install dependencies:
```
pip install -e .
```

Load API keys into the environment for web search:
```
export TAVILY_API_KEY=<your_tavily_api_key>
```

Launch the agent:
```
langgraph dev
```

If all is well, you should see the following output:
```
Ready!

API: http://127.0.0.1:2024
Docs: http://127.0.0.1:2024/docs
LangGraph Studio Web UI: https://smith.langchain.com/studio/?baseUrl=http://127.0.0.1:2024
```

Open `LangGraph Studio Web UI` via the URL in the output. 

In the `configuration` tab:
* You can set the name of your local LLM (it will by default be `llama3.1`) 
* You can set the depth of the research iterations (it will by default be `3`)

Given the agent a topic for research!

## How it works

Research Rabbit is a  AI-powered research assistant that:
- Conducts iterative web research on any given topic
- Generates targeted search queries
- Summarizes findings from multiple sources
- Identifies knowledge gaps and explores them automatically
- Creates comprehensive research summaries with cited sources

## Features

- **Autonomous Research**: Continues down the research rabbit hole through multiple iterations
- **Local LLM Integration**: Uses local LLMs via Ollama (supports llama2/3)
- **Web Search**: Integrates with Tavily API for accurate web search results
- **Smart Summarization**: Incrementally builds knowledge while avoiding redundancy
- **Source Management**: Automatically deduplicates and formats source citations
- **Configurable Depth**: Customizable research iteration depth


