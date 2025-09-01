# custom-AI
# BackendAI Flask App

A Flask web application that interfaces with a local language model API for streaming responses.

## Features
- Real-time streaming responses
- Conversation history (last 5 prompts)
- Simple web interface

## Setup
1. Install dependencies:
   ```
   pip install flask requests waitress
   ```

2. Make sure your language model is running at `http://localhost:11434/api/generate`

3. Run the app:
   ```
   python app.py
   ```

## Production Deployment
```
waitress-serve --port=8000 app:app
```
