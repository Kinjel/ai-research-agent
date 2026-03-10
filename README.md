# AI Research Agent with Web Search

## Overview

This project implements an autonomous **AI research agent** capable of deciding whether to answer a question directly or perform a web search to gather additional information.

The system uses a **Large Language Model (LLM)** to reason about the problem, choose actions, retrieve information from the web, and generate a final answer.

---

## Technologies Used

* Python
* OpenAI API
* DuckDuckGo Search API
* PocketFlow (workflow orchestration)
* YAML (structured decision output)

---

## Features

* Autonomous decision-making using an LLM
* Web search integration for information retrieval
* Iterative research loop for gathering evidence
* Modular workflow using agent nodes

---

## Agent Workflow

1. User provides a question.
2. The LLM analyzes the question and decides the next action.
3. The agent either:

   * performs a web search, or
   * generates a direct answer.
4. Retrieved search results are added to the context.
5. The agent generates a final answer using the gathered information.

---

## Example Question

```id="agent_example_query"
Who won the Nobel Prize in Physics 2024?
```

The agent performs a web search, retrieves relevant information, and generates a final answer.

---

## How to Run

1. Install dependencies

```id="agent_install"
pip install openai
pip install duckduckgo-search
pip install pocketflow
pip install aiohttp
```

2. Add your OpenAI API key.

3. Run the notebook:

```id="agent_run"
ai-research-agent.ipynb
```
