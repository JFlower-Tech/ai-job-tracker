# ai-job-tracker
AI-Powered Job Application Tracker built with Python, FastAPI, Streamlit, and OpenAI API

# 🤖 AI-Powered Job Application Tracker

> A full-stack Python application that helps job seekers track applications and receive AI-generated insights using OpenAI's API.

[![Python](https://img.shields.io/badge/Python-3.11-blue.svg)](https://www.python.org/)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.109.0-green.svg)](https://fastapi.tiangolo.com/)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.30.0-red.svg)](https://streamlit.io/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-16-blue.svg)](https://www.postgresql.org/)

## 🎯 Project Overview

This project showcases modern Python development skills for **Backend Engineering** and **ML/AI Engineering** roles:

- **Backend API**: RESTful API built with FastAPI
- **Frontend Dashboard**: Interactive UI using Streamlit
- **AI Integration**: OpenAI API for intelligent insights
- **Database**: PostgreSQL for data persistence
- **Architecture**: Clean separation of concerns with modular design

## ✨ Features

- 📝 **CRUD Operations**: Create, read, update, and delete job applications
- 🤖 **AI-Powered Insights**: Generate interview prep tips and company insights using OpenAI
- 📊 **Interactive Dashboard**: Visualize application status, timelines, and statistics
- 🔍 **Smart Filtering**: Search and filter applications by status, date, company
- 📈 **Analytics**: Track application success rates and response times

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| **Python 3.11** | Core language (95% of codebase) |
| **FastAPI** | REST API backend framework |
| **Streamlit** | Frontend dashboard & visualization |
| **PostgreSQL** | Relational database |
| **SQLAlchemy** | ORM for database operations |
| **OpenAI API** | AI-powered insights generation |
| **Pydantic** | Data validation & settings |
| **pytest** | Testing framework |

## 🚀 Getting Started

### Prerequisites

- Python 3.11+
- PostgreSQL 16+
- OpenAI API Key

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/JFlower-TechI/ai-job-tracker.git
   cd ai-job-tracker
   ```

2. **Create virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Set up environment variables**
   ```bash
   cp .env.example .env
   # Edit .env with your database and OpenAI API credentials
   ```

5. **Initialize database**
   ```bash
   # Create PostgreSQL database
   createdb job_tracker
   
   # Run migrations
   python backend/app/database.py
   ```

6. **Run the application**
   
   **Backend (Terminal 1):**
   ```bash
   cd backend
   uvicorn app.main:app --reload
   ```
   
   **Frontend (Terminal 2):**
   ```bash
   cd frontend
   streamlit run app.py
   ```

7. **Access the application**
   - Backend API: http://localhost:8000
   - API Docs: http://localhost:8000/docs
   - Frontend: http://localhost:8501

## 📁 Project Structure

```
ai-job-tracker/
├── backend/          # FastAPI backend
├── frontend/         # Streamlit frontend
├── database/         # SQL schema and migrations
└── tests/           # Unit and integration tests
```

## 🧪 Testing

```bash
# Run all tests
pytest

# Run with coverage
pytest --cov=backend --cov=frontend --cov-report=html
```

## 🐳 Docker (Optional)

```bash
# Start all services
docker-compose up -d

# View logs
docker-compose logs -f

# Stop services
docker-compose down
```

## 📚 API Documentation

Once the backend is running, visit:
- Swagger UI: http://localhost:8000/docs
- ReDoc: http://localhost:8000/redoc

### Key Endpoints

- `POST /api/applications/` - Create new job application
- `GET /api/applications/` - List all applications
- `GET /api/applications/{id}` - Get specific application
- `PUT /api/applications/{id}` - Update application
- `DELETE /api/applications/{id}` - Delete application
- `POST /api/ai-insights/{id}` - Generate AI insights for application

## 🎨 Screenshots

_Coming soon_

## 🔮 Future Enhancements

- [ ] Email notifications for application deadlines
- [ ] Chrome extension for one-click application tracking
- [ ] Resume parser using NLP
- [ ] Job matching recommendations using ML
- [ ] Integration with LinkedIn API
- [ ] Mobile app using Flutter

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👤 Author

**JFlower-TechI**

- GitHub: [@JFlower-TechI](https://github.com/JFlower-TechI)
- LinkedIn: [Your LinkedIn]

## 🙏 Acknowledgments

- OpenAI for the GPT API
- FastAPI and Streamlit communities for excellent documentation
- Job seekers everywhere - this tool is for you!

---

⭐ If you find this project helpful, please give it a star!
