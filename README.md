# Conversational AI Toolkit

## Project Overview

This repository contains a Conversational AI Toolkit developed as a
submission for an internship assignment. The project demonstrates core
capabilities of large language models (LLMs) using the Groq API with its
OpenAI SDK compatibility, without relying on any external frameworks.

The toolkit addresses two key tasks:

1.  **Conversation Management & Summarization**: Efficiently manages
    conversation history by summarizing long chats and truncating
    messages to maintain a concise and relevant context.

2.  **Structured Information Extraction**: Uses OpenAI-compatible
    function calling to classify user chats and extract specific data
    points into a structured JSON format.

## Key Features

-   **Stateful Conversation Management**: Maintains a running history of
    user-assistant interactions.
-   **Intelligent Summarization**: Periodically summarizes the
    conversation history to save context and optimize API calls.
-   **History Truncation**: Supports limiting conversation history by
    the number of turns to prevent it from becoming too long.
-   **JSON Schema-based Extraction**: Extracts structured data (e.g.,
    name, email, phone) from unstructured text using a predefined
    schema.
-   **Robust Error Handling**: Gracefully handles scenarios where the
    model does not require function calling, defaulting to a standard
    text response.

## Getting Started

1.  **Clone the Repository**

``` bash
git clone https://github.com/Jaswanth-aditya/Conversational-AI-Toolkit-.git
cd Conversational-AI-Toolkit-
```

2.  **Install Dependencies**\
    This project only requires the openai Python library, which is
    compatible with the Groq API.

``` bash
pip install openai
```

3.  **Set Up Your API Key**\
    To run the notebook, you need a Groq API key:

-   Go to the Groq Console and create a new API key.
-   Open the Google Colab notebook (conversational-toolkit.ipynb).
-   Click on the "🔑" icon on the left-hand side (or select "Secrets"
    from the menu).
-   Add a new secret with the name `GROQ_API_KEY` and paste your API key
    as the value.
-   Ensure "Notebook access" is enabled.

## Project Structure

    Conversational-AI-Toolkit-/
    │
    ├── conversational-toolkit.ipynb       # Main Google Colab notebook
    ├── README.md                      # Project description and instructions
    └── requirements.txt               # Python dependencies

## Usage

Open the `conversational-toolkit.ipynb` file in Google Colab. The notebook
is fully self-contained and provides step-by-step instructions. Run the
cells sequentially to see the demonstration of both Task 1 and Task 2.


