# AccentFlow: Real-Time Accent Changer

## Overview
AccentFlow is a real-time accent conversion application that captures live audio, transcribes it into text using Google Web Speech API, and converts it into a specified accent using AWS Polly’s neural text-to-speech capabilities. This app is built using Python with a simple and interactive web interface created using Streamlit.

## Features
- **Real-Time Speech Transcription**
- **Accent Conversion using AWS Polly**
- **Interactive and User-Friendly Web Interface**
- **Real-Time Feedback and Status Updates**

## Requirements
To run AccentFlow on your local machine, ensure the following requirements are met:

1. **Python 3.7 or higher** installed.
2. **Libraries and Dependencies**:
   - `streamlit`
   - `boto3`
   - `pyaudio`
   - `SpeechRecognition`
3. **Audio Input**: Ensure your system has a microphone attached or supports audio input.

## Installation Guide
### 1. **Clone the Repository**
```bash
git clone https://github.com/your-repository-url
cd your-repository-folder
