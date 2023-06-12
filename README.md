# Chainlit LLM Application

Official URL: https://github.com/Chainlit/chainlit

## Overview
Chainlit is a powerful tool designed to expedite the development of Python Language Learning Model (LLM) applications. This open-source project stands out for its unique ability to seamlessly integrate AI models into applications, providing a streamlined approach for LLM-based applications.

## Usage
The provided script demonstrates the creation of an LLM application using Chainlit. It leverages OpenAI's GPT-3.5 model and the SerpAPI for search functionality.

The script retrieves API keys for OpenAI and SerpAPI from environment variables. It's crucial to ensure these keys are correctly set in your environment before running the script.

A factory function is defined using the @cl.langchain_factory decorator. This function sets up a SerpAPIWrapper instance and a list of tools. Each tool is represented by a Tool instance, which encapsulates a name, a function, and a description.

An instance of OpenAI is created within the factory function, which is then used, along with the list of tools, to initialize an agent using the initialize_agent function. The agent is set up with a specific agent type ('chat-zero-shot-react-description'), and verbosity is set to True.

The factory function returns the initialized agent, which forms the core of the LLM application.
