# 🚀 TS-Forecast AI: Scientific Foundation Model for Multi-Domain Time-Series Forecasting

> **"Where Cutting-Edge AI Meets Real-World Forecasting – Making Scientific Time-Series Prediction Accessible to Everyone"**

[![Python Version](https://img.shields.io/badge/Python-3.10%2B-blue)](https://www.python.org/)
[![PyTorch](https://img.shields.io/badge/PyTorch-2.0%2B-red)](https://pytorch.org/)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.100%2B-green)](https://fastapi.tiangolo.com/)
[![React](https://img.shields.io/badge/React-18.0%2B-blue)](https://reactjs.org/)
[![License](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)
[![Code Style](https://img.shields.io/badge/Code%20Style-Black-black)](https://github.com/psf/black)
[![PRs Welcome](https://img.shields.io/badge/PRs-Welcome-brightgreen)](https://github.com/vishakha2121/TS-Foundation-Multi-Domain-Time-Series-Forecasting-with-Transformer-AI/pulls)

---

## 📋 **Table of Contents**

- [Overview](#-overview)
- [Key Features](#-key-features)
- [Architecture](#-architecture)
- [Domains Supported](#-domains-supported)
- [Technology Stack](#-technology-stack)
- [Quick Start](#-quick-start)
- [Installation Guide](#-installation-guide)
- [Usage Guide](#-usage-guide)
- [Model Training](#-model-training)
- [API Documentation](#-api-documentation)
- [Frontend UI](#-frontend-ui)
- [Gemini AI Integration](#-gemini-ai-integration)
- [Project Structure](#-project-structure)
- [Contributing](#-contributing)
- [License](#-license)
- [Contact](#-contact)

---

## 🌟 **Overview**

**TS-Forecast AI** is an advanced, transformer-based foundation model designed to revolutionize time-series forecasting across multiple critical domains including **industrial sensors**, **financial markets**, **weather patterns**, and **energy consumption**. Built on cutting-edge architectures like **PatchTST** and **Chronos**, this project demonstrates the power of deep learning in predicting complex temporal patterns.

### 🎯 **Why This Project?**

- **No GPU Required**: Optimized for CPU training and inference
- **Beautiful UI**: Enterprise-grade React frontend with modern design
- **Multi-Domain**: Single model for multiple forecasting scenarios
- **Explainable AI**: Understand why predictions are made
- **Gemini AI Integration**: Natural language interaction and insights
- **Real-Time**: Instant visual feedback and interactive charts

---

## ✨ **Key Features**

### 🤖 **Advanced AI Models**
- **PatchTST**: State-of-the-art transformer variant with patch-based attention
- **Chronos**: Pre-trained foundation model with few-shot learning
- **Standard Transformer**: Baseline model for comparison
- **CPU Optimized**: Efficient training and inference on standard hardware

### 📊 **Multi-Domain Support**
- 🏭 **Industrial Sensors**: Temperature, Pressure, Vibration, RPM
- 💰 **Financial**: Stock Prices, Forex, Trading Volume
- 🌤️ **Weather**: Temperature, Humidity, Precipitation, Wind
- ⚡ **Energy**: Power Consumption, Solar Output, Wind Generation

### 🎨 **Modern UI/UX**
- Interactive dashboard with real-time charts
- Drag-and-drop file upload (CSV, Excel, JSON)
- Dark/Light mode toggle
- Responsive design for all devices
- Animated transitions and loading states

### 🔍 **Explainable AI**
- Attention visualization
- Confidence intervals for predictions
- Feature importance analysis
- Model comparison tools

### 🤝 **Gemini AI Integration**
- Natural language insights generation
- Interactive Q&A about predictions
- Automated pattern analysis
- Intelligent data interpretation

---

## 🏗️ **Architecture**

---

## 🎯 **Domains Supported**

| Domain | Data Types | Use Cases |
|--------|------------|-----------|
| 🏭 **Industrial** | Temperature, Pressure, Vibration, RPM, Flow Rate | Predictive Maintenance, Quality Control, Anomaly Detection |
| 💰 **Financial** | Stock Prices, Forex, Trading Volume, Market Indices | Investment Strategies, Risk Assessment, Market Analysis |
| 🌤️ **Weather** | Temperature, Humidity, Precipitation, Wind Speed | Weather Prediction, Climate Research, Agriculture |
| ⚡ **Energy** | Power Consumption, Solar Output, Wind Generation | Smart Grid, Energy Management, Load Forecasting |

---

## 🛠️ **Technology Stack**

### Backend
```python
🐍 Python 3.10+         # Primary language
🚀 FastAPI              # API framework
🧠 PyTorch (CPU)       # Deep learning
📊 Pandas/NumPy        # Data manipulation
🗄️ SQLAlchemy          # ORM
📦 SQLite              # Database
🤖 Gemini API          # AI integration
🐳 Docker              # Containerization

# 1. Clone the repository
git clone https://github.com/vishakha2121/TS-Foundation-Multi-Domain-Time-Series-Forecasting-with-Transformer-AI.git
cd TS-Foundation-Multi-Domain-Time-Series-Forecasting-with-Transformer-AI

# 2. Setup Backend
cd backend
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
cp .env.example .env
# Edit .env with your Gemini API key

# 3. Setup Database
python scripts/setup_database.py

# 4. Start Backend Server
uvicorn app.main:app --reload --host 0.0.0.0 --port 8000

# 5. Setup Frontend (New Terminal)
cd ../frontend
npm install
cp .env.example .env

# 6. Start Frontend
npm run dev

# 7. Open Browser
# Frontend: http://localhost:5173
# Backend API: http://localhost:8000/docs

# 1. Navigate to backend directory
cd backend

# 2. Create virtual environment
python -m venv venv

# 3. Activate virtual environment
# On macOS/Linux:
source venv/bin/activate
# On Windows:
venv\Scripts\activate

# 4. Install dependencies
pip install --upgrade pip
pip install -r requirements.txt

# 5. Environment variables
cp .env.example .env
# Add your Gemini API key: GEMINI_API_KEY=your_key_here

# 6. Initialize database
python scripts/setup_database.py

# 7. Seed sample data
python scripts/seed_database.py

# 8. Run server
uvicorn app.main:app --reload --host 0.0.0.0 --port 8000


# 1. Navigate to frontend directory
cd frontend

# 2. Install dependencies
npm install

# 3. Environment variables
cp .env.example .env
# Set VITE_API_URL=http://localhost:8000

# 4. Run development server
npm run dev

# 5. Build for production
npm run build

# 6. Preview production build
npm run preview