# Sample-modular-genai-app

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
