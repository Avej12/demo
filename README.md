Log Analysis System
AI-powered cybersecurity log analysis system with automated threat detection, cross-endpoint correlation, and incident reporting.
Environment Setup
Create virtual environment:
bashpython -m venv .venv
Activate environment:
bash.venv/Scripts/activate
Install dependencies:
bashpip install -r requirements.txt
Configuration
Create .env file:
envGEMINI_API_KEY=your_gemini_api_key
OPENSEARCH_HOST=your_opensearch_host
OPENSEARCH_PORT=9200
OPENSEARCH_USERNAME=your_username
OPENSEARCH_PASSWORD=your_password
LOG_LEVEL=INFO
Running the System
Terminal 1 - Flask Backend
bashpython app.py

Runs on http://localhost:5000
Processes logs via queue system
Provides REST API endpoints

Terminal 2 - Streamlit Dashboard
bashstreamlit run streamlit_app.py

Runs on http://localhost:8501
Real-time monitoring dashboard
