# ai-job-tracker
AI-Powered Job Application Tracker built with Python, FastAPI, Streamlit, and OpenAI API



ai-job-tracker/
├── .github/
│   └── workflows/
│       └── ci.yml                 # GitHub Actions for CI/CD
├── backend/
│   ├── app/
│   │   ├── __init__.py
│   │   ├── main.py               # FastAPI app entry point
│   │   ├── models.py             # Database models
│   │   ├── schemas.py            # Pydantic schemas
│   │   ├── database.py           # Database connection
│   │   ├── crud.py               # CRUD operations
│   │   └── routers/
│   │       ├── __init__.py
│   │       ├── applications.py   # Job application endpoints
│   │       └── ai_insights.py    # AI-powered endpoints
│   ├── tests/
│   │   ├── __init__.py
│   │   └── test_api.py
│   ├── requirements.txt
│   └── .env.example
├── frontend/
│   ├── app.py                    # Streamlit main app
│   ├── pages/
│   │   ├── 1_📊_Dashboard.py
│   │   ├── 2_➕_Add_Application.py
│   │   └── 3_🤖_AI_Insights.py
│   ├── components/
│   │   ├── __init__.py
│   │   └── charts.py
│   ├── requirements.txt
│   └── .streamlit/
│       └── config.toml
├── database/
│   ├── init.sql                  # Database schema
│   └── seed.sql                  # Sample data (optional)
├── .gitignore
├── .env.example
├── README.md
├── requirements.txt              # Root level dependencies
├── docker-compose.yml            # For easy local setup
└── setup.py                      # For package installation
