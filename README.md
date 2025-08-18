## 🐍 uv

### What is it?

- Ultra-fast Python package & virtual environment manager (pip/poetry alternative)
- Built in Rust, automatically manages virtual environments

### Installation (macOS)

- Install with Homebrew: `brew install uv`
- Verify: `uv --version`

### Usage

- Add a package: `uv add requests`
- Run: `uv run python app.py` / Sync: `uv sync`

---

## 🔗 LangChain vs LangGraph

### LangChain

- **Components**: Provides modules such as `PromptTemplate`, `LLM`, `Tool`, `Memory`, `Retriever`
- **Chains**: Connect multiple components in a sequential pipeline
- **Agents**: Allow the LLM to dynamically decide which `Tools` to call
- **Main Purpose**: A framework to quickly build LLM-powered applications

### LangGraph

- **Graph**: Execution flow composed of `Nodes` (agents or chains) and `Edges` (execution paths)
- **Conditional Edges**: Enable branching based on results
- **Cycles**: Allow loops to repeat or go back to previous nodes
- **Concurrency**: Support parallel execution of multiple nodes
- **Main Purpose**: An engine for defining and running complex multi-agent workflows

### Summary

- **LangChain** → A framework for creating `Chains` and `Agents`
- **LangGraph** → An engine for organizing those `Chains/Agents` as `Nodes` in a `Graph` workflow and executing them

## ⚙️ Virtual Environment with uv

### Create venv

```
uv venv
```

### Activate venv

```
source .venv/bin/activate
```

### Deactivate venv

```
deactivate
```
