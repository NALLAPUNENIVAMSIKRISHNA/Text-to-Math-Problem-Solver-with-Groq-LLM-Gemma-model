# Groq Powered Math, Reasoning, and Wikipedia Agent

This Streamlit application combines the power of the Groq LLM with LangChain to create a versatile agent capable of solving math problems, answering reasoning questions, and retrieving information from Wikipedia.

## Features

* **Math Problem Solving:** Solves mathematical problems using natural language input.
* **Logical Reasoning:** Answers logic-based and reasoning questions with detailed explanations.
* **Wikipedia Search:** Retrieves information from Wikipedia based on user queries.
* **Groq LLM Powered:** Utilizes the fast Groq LLM for quick and accurate responses.
* **Interactive Streamlit Interface:** User-friendly web interface for easy interaction.
* **Agent Tooling:** Utilizes LangChain agents and tools for versatile question handling.
* **Detailed Reasoning:** The agent shows its reasoning process step by step.

## Getting Started

### Prerequisites

* Python 3.7+
* A Groq API key (We will get from Groq cloud website)
* Internet connection

### Installation

1.  **Clone the repository**

2.  **Create a virtual environment**

3.  **Install dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

4.  **Run the application:**

    ```bash
    streamlit run app.py
    ```

### Usage

1.  **Enter Groq API Key:**
    * In the sidebar, enter your Groq API key.
2.  **Enter Question:**
    * In the main interface, enter your math problem, reasoning question, or Wikipedia search query.
3.  **Find Answer:**
    * Click the "find my answer" button.
4.  **View Response:**
    * The agent's response, including detailed explanations and reasoning steps, will be displayed.

### Code Explanation

* **`app.py`:**
    * This file contains the Streamlit application and the LangChain agent setup.
    * It initializes the Groq LLM, defines tools (Wikipedia, Calculator, Reasoning), and sets up the agent.
    * It handles user input and displays the agent's responses.

### Dependencies

* `streamlit`
* `langchain`
* `langchain-groq`
* `langchain-community`

### Agent Tools

* **Wikipedia Tool:** Uses `WikipediaAPIWrapper` to search Wikipedia.
* **Calculator Tool:** Uses `LLMMathChain` to solve math problems.
* **Reasoning Tool:** Uses `LLMChain` with a custom prompt to answer logical reasoning questions.
