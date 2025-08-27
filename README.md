# Log Analysis System

AI-powered cybersecurity log analysis system with automated threat detection, cross-endpoint correlation, and incident reporting.

## Environment Setup

### Create virtual environment:

python -m venv .venv

### Activate environment:

.venv/Scripts/activate

### Install dependencies:

pip install -r requirements.txt

### Configuration

#### Create .env file:

##### GEMINI_API_KEY=your_gemini_api_key
##### OPENSEARCH_HOST=your_opensearch_host
##### OPENSEARCH_PORT=9200
##### OPENSEARCH_USERNAME=your_username
##### OPENSEARCH_PASSWORD=your_password

## Running the System
### Terminal 1 - Flask Backend
python app.py

Runs on http://localhost:5000
Processes logs via queue system
Provides REST API endpoints

### Terminal 2 - Streamlit Dashboard
streamlit run streamlit_app.py

Runs on http://localhost:8501
Real-time monitoring dashboard

## Critical alerts should be sent to http://localhost:5000/logs API endpoint for automated analysis and threat detection.
