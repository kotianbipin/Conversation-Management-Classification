# Conversation Management & Classification using Groq API

## Objective
This assignment demonstrates two core tasks using the Groq API with OpenAI SDK compatibility:
1. **Conversation Management and Summarization**: Maintaining a running conversation history, performing periodic summarization, and truncation based on conversation turns or character/word limits.
2. **JSON Schema Classification & Information Extraction**: Extracting structured user information (name, email, phone, location, age) using function calling with the Groq API.

---

## Repository Contents
- `Conversation_Management_and_Extraction.ipynb` – Main Colab notebook implementing all tasks.
- `README.md` – This file describing the project.

---

## Requirements
- Python 3.x
- Google Colab
- Groq API key (stored securely using Colab Secrets; not hardcoded)
- `openai` Python package (used for Groq OpenAI-compatible SDK)

---

## Features

### Task 1: Conversation Management & Summarization
- Maintains running conversation history.
- Supports truncation:
  - Limit by number of conversation turns.
  - Limit by character/word length.
- Performs **periodic summarization** after every k-th conversation run.
- Demonstrated with multiple sample conversations.

### Task 2: JSON Schema Classification & Information Extraction
- Extracts 5 key user details from chats: `name`, `email`, `phone`, `location`, `age`.
- Uses **function calling** for structured outputs.
- Includes validation against the JSON schema.
- Demonstrated with 3 sample chat examples:
  - Complete information
  - Partial information
  - Mixed information

---

## How to Use
1. Open the notebook in **Google Colab**.
2. Set your **Groq API key** via Colab Secrets:
   - Click **Files → Secrets (🔒)** and add `GROQ_API_KEY`.
3. Run the notebook cells sequentially:
   - **CELL 2**: Load API key and test Groq connection.
   - **Other cells**: Conversation management, summarization, extraction, and validation.
4. Review outputs and extraction results.

---

## References
- [Groq API Documentation](https://console.groq.com/docs/openai)
- [OpenAI Function Calling Guide](https://platform.openai.com/docs/guides/function-calling)


