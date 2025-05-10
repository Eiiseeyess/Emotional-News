# Sentiment-Driven News Aggregator

A project to collect news from Kenyan sources (initially The Standard), analyze sentiment, and provide voice-interactive summaries.

## Project Overview

*   **Sentiment-Driven News Aggregator**: Collects news articles, analyzes their sentiment (positive, negative, neutral), and organizes them accordingly.
*   **Voice-Interactive News Summarizer**: Allows users to interact with the news via voice commands and hear audio responses on their summaries .

## Tech Stack

*   **Programming Language**: Python
*   **News Collection**: `feedparser`
*   **Sentiment Analysis**: `VADER (Valence Aware Dictionary and sEntiment Reasoner)`
*   **Summarization**: `spaCy`
*   **Voice Interaction**:
    *   `SpeechRecognition` (with Google Speech Recognition engine)
    *   `gTTS` (Google Text-to-Speech)
*   **Web Interface**: `Flask`
*   **Database**: `SQLite`
*   **Workflow Automation**: `n8n` (planned)

## Setup

1.  **Create a virtual environment (recommended):**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```

2.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

3.  **Download spaCy model:**
    ```bash
    python -m spacy download en_core_web_sm
    ```

4.  **Run the application (details to be added as development progresses).**

## Directory Structure

-   `data/`: Stores the SQLite database (`news.db`).
-   `scripts/`: Contains Python scripts for various tasks:
    -   `fetch_news.py`: Fetches news articles from RSS feeds.
    -   `sentiment_analysis.py`: Analyzes sentiment of fetched articles.
    -   `summarize_news.py`: Generates summaries for articles.
-   `webapp/`: Contains the Flask web application.
    -   `app.py`: Main Flask application file.
    -   `templates/`: HTML templates for the web interface.
    -   `static/`: (Optional) CSS, JavaScript files.
-   `requirements.txt`: Project dependencies.
-   `README.md`: This file. 