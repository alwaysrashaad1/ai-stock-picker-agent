# AI Stock Picker – Multi-Agent Investment Recommendation System

## Overview

AI Stock Picker is a multi-agent system designed to identify trending companies, research their financials, and select high-potential stocks. Built with Python, LangChain, and various AI agents, it leverages GPT-5-mini for natural language reasoning and decision-making, enabling data-driven investment recommendations.

The system is modular, allowing you to extend or customize agents for different research strategies, sources, or financial goals.

## Features

* **Trending Company Discovery:** An agent scans news, social media, and financial sources to identify trending companies.
* **Financial Research:** An agent analyzes company financials, news, and market sentiment.
* **Stock Selection:** A decision-making agent evaluates potential investments based on the research results.
* **Multi-Agent Architecture:** Each agent has a clearly defined role, enabling scalability and experimentation.
* **JSON & SQLite Integration:** Structured output allows easy storage, retrieval, and further analysis of investment data.
* **Prompt Optimization:** Carefully designed prompts improve accuracy, reasoning, and consistency of the agents’ outputs.

## Files

* `main.py` (or entrypoint file): Runs the AI Stock Picker and orchestrates agents.
* `agents/` folder: Contains modules for each AI agent (trending company, research, stock selection).
* `prompts/` folder: Contains prompt templates used for reasoning, evaluation, and data extraction.
* `utils.py`: Helper functions for data processing, API calls, and formatting.
* `database.db` (optional): SQLite database for storing stock data and research results.

## Installation

1. Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPO.git
cd YOUR_REPO
```

2. Create and activate a virtual environment:

```bash
python -m venv .venv
source .venv/bin/activate   # Linux/Mac
.venv\Scripts\activate      # Windows
```

3. Install dependencies:

```bash
pip install -r requirements.txt
```

4. Add any required API keys in a `.env` file:

```env
SERPER_API_KEY=your_serper_key
PUSHOVER_TOKEN=your_pushover_token
PUSHOVER_USER=your_pushover_user
```

## Usage

1. Run the main script to start the multi-agent workflow:

```bash
python main.py
```

2. Agents will:

   * Identify trending companies
   * Research company financials
   * Evaluate and select top stocks

3. Output will be stored in structured JSON or SQLite, depending on your configuration.

