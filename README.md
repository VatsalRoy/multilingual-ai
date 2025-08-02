# Multilingual AI 🌍🎙️

A Python-based AI assistant that processes YouTube video audio and answers questions in multiple languages using AssemblyAI's LeMUR and Claude 3.5 Sonnet.

## Features ✨
- 📥 Downloads audio from YouTube videos with `yt-dlp`.
- 🎤 Transcribes audio using AssemblyAI.
- ❓ Answers questions in specified languages (e.g., Spanish) via LeMUR.
- 📚 Example: Analyzes Steve Jobs' 2005 Stanford Commencement Address.

## Prerequisites 🛠️
- Python 3.10+
- FFmpeg
- AssemblyAI API key
- Internet connection

## Installation 🚀
1. Install FFmpeg:
   ```bash
   sudo apt-get install ffmpeg
   ```
2. Install Python packages:
   ```bash
   pip install yt-dlp assemblyai
   ```
3. Set AssemblyAI API key:
   ```python
   import assemblyai as aai
   aai.settings.api_key = "your-api-key"
   ```

## Usage ▶️
1. Open `multilingual_ai.ipynb` in Jupyter or Colab.
2. Set YouTube URL:
   ```python
   URL = "https://www.youtube.com/watch?v=your-video-id"
   ```
3. Define question prompt:
   ```python
   prompt = "What are the 5 key messages in the speech? Please explain in Spanish."
   ```
4. Run the notebook to download, transcribe, and get answers.

## Example 📖
Processes `https://www.youtube.com/watch?v=UF8uR6Z6KLc` and answers in Spanish:
```
Basado en el discurso de Steve Jobs, los 5 mensajes clave son:
1. Confía en que los puntos se conectarán en el futuro
...
```

## Project Structure 📂
- `multilingual_ai.ipynb`: Main notebook.
- Temporary audio files: `{video_title}.mp3`.

## Dependencies 📦
- `yt-dlp`: YouTube audio downloader.
- `assemblyai`: Transcription and Q&A.
- `ffmpeg`: Audio processing.

## Notes 📝
- Ensure a valid AssemblyAI API key.
- Designed for Colab but adaptable for local use.
- Avoid unnecessary file I/O or network calls.

## References 🔗
- [LeMUR Docs](https://www.assemblyai.com/docs/lemur)
- [Ask Questions](https://www.assemblyai.com/docs/lemur/ask-questions)
- [AssemblyAI Cookbook](https://github.com/AssemblyAI/cookbook/blob/master/lemur/using-lemur.ipynb)
