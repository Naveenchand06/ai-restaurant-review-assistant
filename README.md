# Local RAG AI Agent — Restaurant Review Assistant

This is a lightweight AI Agent that runs locally using Ollama, ChromaDB, and LangChain.
It uses RAG (Retrieval Augmented Generation) to answer questions about restaurant reviews stored in a CSV file!

### 🚀 How It Works

- Embeds the restaurant reviews from `restaurant_reviews.csv` into a local Chroma vector database.
- Retrieves the most relevant reviews based on your question.
- Uses a local LLM (through Ollama) to generate answers using the retrieved reviews as context.

### ⚙️ Setup Instructions

Clone the repository:

```
git clone https://github.com/Naveenchand06/restaurant-review-assistant.git
cd restaurant-review-assistant

Install dependencies:
pip install -r requirements.txt
```

Make sure Ollama is running locally.
You can download and run Ollama models from Ollama.
Prepare your CSV:
The file `restaurant_reviews.csv` should have at least these columns:
_Title_
_Review_
_Rating_
_Date_

Run the application:

```
python3 main.py
```

Start chatting!

Ask any questions related to the restaurant.
Example:
"What do customers say about the pizza crust?"

### 🛠 Tech Stack

LangChain — Chains, Prompts, and Document Retrieval
Ollama — Local LLM models (like Llama3, Mistral)
ChromaDB — Lightweight local Vector Database
Python — Core language for scripting
