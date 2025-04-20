# Sample-modular-genai-app


# 🧠 GenAI Application Stack

A modular, multi-provider GenAI application that supports tasks like document validation, summarization, and retrieval-augmented generation (RAG) using configurable backends like OpenAI, AWS Bedrock, Azure OpenAI, and more.


---

## 📁 Project Structure
```
Sample-modular-genai-app/
├── genai_app/
│   ├── api/
│   │   ├── main.py
│   │   ├── routes/
│   │   ├── services/
│   │   │   └── tasks/
│   │   │       ├── validator.py
│   │   │       ├── summarizer.py
│   │   │       └── rag_handler.py
│   │   └── schemas/
│   ├── llm_providers/
│   │   ├── base.py
│   │   ├── openai_provider.py
│   │   ├── bedrock_provider.py
│   │   └── azure_openai_provider.py
│   ├── models/
│   │   ├── prompts/
│   │   │   ├── validate_property.txt
│   │   │   ├── summarize_property.txt
│   │   │   └── config.yaml
│   │   └── rag/
│   │       ├── rag_pipeline.py
│   │       └── vector_store.py
│   ├── config/
│   │   ├── settings.py
│   │   └── logging.yaml
│   ├── ui/
│   │   └── app.py
│   ├── utils/
│   │   ├── pdf_extractor.py
│   │   └── formatter.py
│   ├── tests/
│   │   ├── test_api.py
│   │   ├── test_ui.py
│   │   └── test_validation_pipeline.py
├── .env
├── requirements.txt
├── run_all.sh
└── README.md
│   ├── test_api.py
│   ├── test_ui.py
│   └── test_validation_pipeline.py
├── .env
├── requirements.txt
├── run_all.sh
└── README.md
```
---

## ✨ Features

- 🔌 Plug-and-play LLM provider interface
- ✅ Task modules for validation, summarization, and RAG
- 🧠 External prompt and RAG configuration
- 📄 Unified backend API with FastAPI
- 🖥️ Optional UI layer via Streamlit
- 🔧 Centralized config and environment management
- 🧪 Tests scaffolded for API, UI, and tasks

## ✨ Features

- 🔌 Multi-provider LLM support (OpenAI, Bedrock, Azure, etc.)
- ✅ Validation pipelines for structured/unstructured docs
- 🧠 RAG support for knowledge-aware reasoning
- 📄 Externalized, versionable prompts
- ⚙️ Configurable settings via `.env` or `settings.py`
- 🧪 Unit test structure included
- 🖥️ Optional Streamlit UI for quick testing

---

## 🚀 Getting Started

```bash
# Clone the repo
git clone https://github.com/your-org/genai-app-stack.git
cd genai-app-stack
```

# Set up virtual environment
python -m venv venv
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Run API
uvicorn api.main:app --reload

# (Optional) Run UI
streamlit run ui/app.py

---



