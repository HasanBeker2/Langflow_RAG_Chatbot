
# RAG-Based LLM Chatbot Application

This repository contains the code and resources needed to build a Retrieval-Augmented Generation (RAG) based chatbot application using LangFlow. This chatbot can answer questions based on the content of a provided PDF document, making it ideal for scenarios such as restaurant FAQs or any other context where common questions are frequently asked.

## Overview

In this project, you'll find all the necessary components to create your own AI application that utilizes RAG without writing a single line of code. The application is built using LangFlow, a visual tool that allows for intuitive connection of pre-built components, enabling the creation and deployment of AI workflows effortlessly.

## Features

- **User Interaction**: The chatbot can accept and respond to user questions.
- **Contextual Responses**: Uses content from a provided PDF to generate relevant responses.
- **Memory Retention**: Remembers conversation history for continuous interaction.
- **Customizable**: Easily import and export flows using JSON files.

## Requirements

- **Python**: Version 3.10 or above.
- **LangFlow**: Installed via pip.
- **Astra DB**: From DataStax for vector storage.
- **OpenAI API Key**: For embedding and generating responses.

## Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/rag-llm-chatbot.git
   cd rag-llm-chatbot
   ```

2. **Install LangFlow**:
   ```bash
   pip install langflow --pre --force-reinstall
   ```

3. **Setup Astra DB**:
   - Create an account on [DataStax Astra](https://www.datastax.com/).
   - Create a serverless vector database.
   - Generate the necessary endpoint and token.

4. **Setup OpenAI API**:
   - Create an account on [OpenAI](https://platform.openai.com/signup).
   - Generate an API key.

## Configuration

1. **Run LangFlow**:
   ```bash
   langflow run
   ```

2. **Load the Flow**:
   - Open your browser and navigate to `localhost` (URL provided by LangFlow upon running).
   - Import the provided `json` file from this repository.
   - Load the PDF document you want to use for the chatbot responses.

3. **Set Environment Variables**:
   - OpenAI API Key
   - Astra DB Endpoint
   - Astra DB Token
   - Collection name for your PDF data

## Usage

1. **Start the Application**:
   - After setting up the flow, click `Run` in LangFlow.
   - Interact with the chatbot by entering your name and asking questions.

2. **Change User**:
   - To change the user and reset the conversation history, simply enter a new name.

## Files

- **`Restaurant Virtual Assistant (without API keys).json`**: The JSON file containing the flow setup for LangFlow.
- **`Resturaunt Q&A.pdf`**: Sample PDF document used for testing.
