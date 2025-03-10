# Financial-Agent-Agentic-Ai-Phidata
Agentic AI - Financial Agent with Phidata

# Multi-AI Financial Analysis Agent

This project implements a multi-agent system for financial analysis, leveraging the power of Google's Gemini model. It combines web search capabilities with real-time financial data retrieval to provide comprehensive insights into stocks and market trends.

## Features

* **Web Search Agent:**
    * Performs targeted web searches for financial information.
    * Verifies source credibility.
    * Provides concise summaries with source links.
* **Financial Agent:**
    * Retrieves stock data using the `yfinance` library.
    * Includes current price, key fundamentals, analyst recommendations, and recent company news.
    * Formats data in tables for readability.
* **Multi-AI Agent:**
    * Orchestrates the web search and financial agents.
    * Combines results into a single, cohesive response.
    * Follows clear formatting guidelines for easy understanding.
    * Uses Gemini 2.0 flash.
* **Enviornment variable usage:**
    * Uses a .env file to store the google api key.

## Installation

1.  **Clone the repository:**

    ```bash
    git clone [repository URL]
    cd [repository directory]
    ```

2.  **Create a virtual environment (recommended):**

    ```bash
    python -m venv venv
    source venv/bin/activate  # On macOS and Linux
    venv\Scripts\activate  # On Windows
    ```

3.  **Install dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

4.  **Set up environment variables:**

    * Create a `.env` file in the project root.
    * Add your Google API key:

        ```
        GOOGLE_API_KEY=your_api_key_here
        ```

5.  **Run the script:**

    ```bash
    python your_script_name.py
    ```
    (Replace your\_script\_name.py with the name of your python file)

## Usage

The `multi_ai_agent` is designed to process user queries related to financial analysis. Here's an example:

```python
multi_ai_agent.print_response(
    "Summarize analyst recommendations and share the latest news for NVIDIA Corporation (NVDA).",
    stream=True,
)

The agent will then:

- Use the web_search_agent to gather relevant news.
- Use the financial_agent to retrieve stock data from yfinance.
- Combine the results and present them in a structured format.

Dependencies:
- phi.agent
- phi.model.google
- phi.tools.yfinance
- phi.tools.duckduckgo
- python-dotenv
- yfinance

Future Improvements:
- Implement more advanced data visualization.
- Add support for other financial data sources.
- Enhance the agent's ability to handle complex queries.
- Add more comprehensive error handling.
- Increase the amount of tools available to the agents.


![image](https://github.com/user-attachments/assets/3294ad25-a7b4-478e-b3ab-784a80f0d282)
![image](https://github.com/user-attachments/assets/60ade67d-bab4-469d-b30a-1bdc1baea798)
![image](https://github.com/user-attachments/assets/b55edd1e-db02-45fb-bc76-f77d57e3af79)


