# AI Chatbot using LangGraph

A conversational AI chatbot built using **LangGraph**, **LangChain**, **Streamlit**, and **Google Gemini (gemini-3-pro-preview)**.

The chatbot supports:
- Conversational memory
- Multiple chat sessions
- Real-time streaming responses
- Context-aware conversations

---

## Demo

![Demo](assets/demo.gif)

---

## Features

### Conversational Memory
The chatbot remembers previous messages within a conversation thread using LangGraph memory.

Example:

```text
User: What is the capital of India?
Bot: New Delhi

User: What about Nepal?
Bot: Kathmandu
```

Even though the second question is incomplete, the chatbot understands the context from previous conversation history.

---

### Multiple Chat Sessions
Users can create and switch between multiple chat conversations during the same session.

Each chat maintains its own independent memory and conversation history.

---

### Real-Time Streaming Responses
Responses are streamed token-by-token in the UI for a more interactive chatbot experience.

---

### Context-Aware AI Responses
The chatbot uses Google's Gemini model through LangChain integration to generate intelligent and contextually relevant responses.

---

## Tech Stack

- **Python**
- **LangGraph**
- **LangChain**
- **Streamlit**
- **Google Gemini API**
- **ChatGoogleGenerativeAI**
- **LLM-based conversational AI**

---

## Project Structure

```text
├── langgraph_backend.py
├── streamlit_frontend_threading.py
├── requirements.txt
├── README.md
└── assets/
    └── demo.gif
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/kanishkagargg/AI-ChatBot-using-LangGraph.git
```

Move into the project directory:

```bash
cd AI-ChatBot-using-LangGraph
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Environment Variables

Create a `.env` file and add your Google API key:

```env
GOOGLE_API_KEY=your_api_key_here
```

---

## Run the Application

```bash
streamlit run streamlit_frontend_threading.py
```

---

## How It Works

- LangGraph manages conversational workflow and memory.
- Streamlit provides the frontend chat interface.
- LangChain connects the application to Gemini LLM.
- Each conversation is associated with a unique `thread_id`.
- Chat history is preserved using LangGraph checkpointer memory.

---

## Future Improvements

- Persistent database memory
- User authentication
- Chat export functionality
- Cloud deployment
- Vector database integration
- RAG-based document chatbot

---

## Author

Kanishka Garg
