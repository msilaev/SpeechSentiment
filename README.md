# SpeechSentiment

**SpeechSentiment** is a web application that enables users to upload text or audio files (MP3) for sentiment analysis. It leverages OpenAI's Whisper model for audio transcription and performs sentiment analysis on the transcribed text or directly on uploaded text files.

---

## Features

- Analyze sentiment in uploaded text files.
- Transcribe audio files (MP3) to text using OpenAI's Whisper model.
- Perform sentiment analysis on the transcribed text.
- Display sentiment analysis results in a user-friendly web interface.

---

## Requirements

- Python 3.7+
- Flask
- OpenAI API key

---

## Installation

1. **Clone the repository**:
   ```sh
   git clone https://github.com/yourusername/SpeechSentiment.git
   cd SpeechSentiment
   ```

2. **Create a virtual environment and activate it**:
   - On Linux/macOS:
     ```sh
     python -m venv venv
     source venv/bin/activate
     ```
   - On Windows:
     ```sh
     python -m venv venv
     venv\Scripts\activate
     ```

3. **Install required packages**:
   ```sh
   pip install -r requirements.txt
   ```

4. **Set up environment variables**:
   - Create a `.env` file in the root directory of the project.
   - Add your OpenAI API key:
     ```env
     OPEN_AI_KEY=your_openai_api_key
     ```

5. **Download sentiment analysis model weights**:
   - Download `model.joblib` and `vectorizer.joblib` into the `/models` folder from this [Google Drive link](https://drive.google.com/file/d/14J1_bRLaMnk9yCbfRdr_8LVT_LicS8Wn/view?usp=sharing).

---

## Usage

1. **Run the Flask application**:
   ```sh
   flask run
   ```

2. **Access the application**:
   - Open your web browser and navigate to:  
     [http://127.0.0.1:5000/](http://127.0.0.1:5000/)

3. **Upload files for analysis**:
   - Upload text or audio files (MP3) and view the sentiment analysis results.

---

## Project Structure

```
SpeechSentiment/
├── .env
├── .gitignore
├── README.md
├── requirements.txt
├── config.py
├── app/
│   ├── __init__.py
│   ├── routes.py
│   ├── templates/
│   │   ├── base.html
│   │   ├── upload.html
│   │   └── result.html
│   └── static/
│       ├── css/
│       └── js/
├── models/
│   ├── model.joblib
│   └── vectorizer.joblib
└── venv/
```

---

## Acknowledgements

- **OpenAI**: For providing the Whisper model and API.
- **Flask**: For the web framework.
- **Bootstrap**: For the front-end framework.

---
