# 🎵 Audio to Sentiment Transcriber

> **Transform audio into transcribed text and sentiment insights instantly!**  
> A powerful Python SDK that leverages AssemblyAI to transcribe audio files and analyze sentiment with high precision.

---

## ✨ Key Features

- **🎙️ High Precision Transcription**: Powered by **AssemblyAI**'s state-of-the-art speech-to-text engine.
- **🧠 Sentiment Analysis**: Gain deep insights into the emotional tone of your audio content.
- **🔍 Advanced Detection**:
  - **Auto Chapters**: Summarize long audio into manageable sections.
  - **Entity Detection**: Automatically identify people, places, and things.
  - **Auto Highlights**: Extract the most important keywords and phrases.
- **⚡ Simple Integration**: Easy-to-use Python functions for seamless workflow integration.

---

## 🛠️ Tech Stack

- **Core**: `requests`, `validators`
- **AI Engine**: `AssemblyAI`
- **Logic**: `Python`

---

## 🚀 Getting Started

### 📋 Prerequisites

You will need an **AssemblyAI API Key**. Get it for free [here](https://app.assemblyai.com/).

### 💻 Local Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/kokilamariyayi/audio-to-sentiment.git
   cd audio-to-sentiment
   ```

2. **Install dependencies:**
   ```bash
   pip install .
   ```

---

## 📖 How to Use

### 1. Set Up Your API Key

```python
import assembly_ai
assembly_ai.api_key = "YOUR_API_KEY"
```

### 2. Transcribe and Get Results

```python
from assembly_ai.walkthroughs import submit_url_for_transcription, get_transcription_results

# Submit audio for transcription with sentiment analysis enabled
response = submit_url_for_transcription(
    audio_url="https://bit.ly/3yxKEIY",
    sentiment_analysis=True
)

# Get the results (waits for completion)
results = get_transcription_results(response['id'], all_details=True)

print(f"Text: {results['text']}")
print(f"Sentiment: {results['sentiment_analysis_results']}")
```

---

## 📁 Project Structure

```bash
audio-to-sentiment/
├── src/
│   └── assembly_ai/        # Core SDK logic
│       ├── __init__.py     # Package entry point
│       ├── walkthroughs.py # Main functions (Transcribe, Results)
│       └── endpoints.py    # API Endpoints
├── pyproject.toml          # Build configuration
├── LICENSE                 # MIT License
└── README.md               # Documentation
```

---

## 📬 Let's Connect

If you found this project useful, feel free to reach out for collaborations or feedback!

- **LinkedIn**: [Kokila M](https://www.linkedin.com/in/kokila-m-ai-ds/)
- **Email**: [kokilakoki3376@gmail.com](mailto:kokilakoki3376@gmail.com)
- **GitHub**: [kokilamariyayi](https://github.com/kokilamariyayi)

---

## 📄 License

Distributed under the **MIT License**. See `LICENSE` for more information.

---
<div align="center">
  <b>Built with ❤️ by Kokila M</b>
</div>
