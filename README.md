# Smart_Audio_Interaction_with_OpenAI

This project integrates **speech recognition**, **OpenAI's GPT-3.5**, and **text-to-speech synthesis** to create an interactive audio-based system.

## Features

- **Speech-to-Text:** Converts audio files into text.
- **AI Response:** Sends text to OpenAI for generating responses.
- **Text-to-Speech:** Converts AI responses into audio and plays it.

## Requirements

- Python 3.x
- `pydub`, `SpeechRecognition`, `pyttsx3`, `openai`
- FFmpeg (for `pydub`)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/audio-processing-with-openai.git
   cd audio-processing-with-openai
2. Install dependencies:
   ```bash
   pip install pydub SpeechRecognition pyttsx3 openai

3. Install FFmpeg:
- Windows: Download FFmpeg
- macOS: brew install ffmpeg
- Linux: sudo apt install ffmpeg

## Usage
1. Set your OpenAI API key in the code.
2. Prepare an audio file.
3. Run:
   ```bash
   python process_audio.py
نسخ
## Troubleshooting
If you encounter the error:
    ```bash
   Error converting audio to text: Audio file could not be read as PCM WAV, AIFF/AIFF-C, or Native FLAC; check if file is corrupted or in another format 
   Failed to process the audio file.

This usually occurs when the audio file format is unsupported. To resolve this:
1. Ensure the audio file is in WAV or FLAC format (PCM encoding).
2. Convert the audio to the correct format using FFmpeg:
    ```bash
    ffmpeg -i input_audio.mp3 output_audio.wav

## Improvements
1. Support for additional audio formats: We plan to add support for more audio formats and error handling improvements.
2. Optimizing performance: Work is underway to enhance the efficiency of audio file processing and OpenAI response time.

