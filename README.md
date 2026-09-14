# AI-tool-calling
# Gemini API: AI Tool-Calling & Agent Routing

A portfolio of lightweight, production-ready Python implementations demonstrating function calling, dynamic intent routing, and parameter guardrails using the Google GenAI SDK

## 🛠 Repository Overview

This repository demonstrates how to bridge LLMs with deterministic Python functions (Tools). Each interactive notebook is configured to run directly in Google Colab using `Gemini_API_Key1` stored securely in Colab Secrets.

### Featured Mini-Projects

| Mini-Project | Key Capabilities | Interactive Notebook |
| **1. Single Tool Execution** | Automatic Function Calling, single-tool docstring parsing, type extraction. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/DuhranDuhran/AI-tool-calling/blob/main/Single_Tool_Execution.ipynb) |
| **2. Multi-Tool Intent Router** | Multi-tool schema evaluation, zero-shot tool selection based on query context. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/DuhranDuhran/AI-tool-calling/blob/main/Multi_Tool_Intent_Router.ipynb) |
| **3. Parameter Guardrails & Error Handling** | Regex email validation, datetime parsing, numerical bound checks, client API error handling. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/DuhranDuhran/AI-tool-calling/blob/main/Guardrails_and_Error_Handling.ipynb) |

## 🚀 Key Architectural Patterns

1. **Automatic Function Calling:** Leverages Gemini's client SDK to auto-execute functions upon model selection and pass results back to the LLM in a single execution turn.
2. **Deterministic Guardrails:** Implements multi-layered input sanitization (`re`, `datetime`, boundary checks) directly inside tools to return informative error strings without crashing the process.
3. **Resilient Execution:** Wraps model generation calls in client-level `try/except` blocks to handle API errors, network issues, and rate limits gracefully.

## 💻 Environment & Setup

1. Clone or open any notebook directly in Google Colab using the **Open in Colab** badges above.
2. Store your API Key in Google Colab:
   * Click the **Key Icon (🔑 Secrets)** in the left sidebar.
   * Add Name: `Gemini_API_Key1`
   * Add Value: `[Your Google AI Studio API Key]`
   * Toggle **Notebook access** to **ON**.
3. Run the notebook cells sequentially.
