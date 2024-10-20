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
```
git clone https://github.com/your-repository-url
cd your-repository-folder
```
### 2. Set Up a Virtual Environment (Optional but recommended)
```
python3 -m venv venv
source venv/bin/activate  # On Windows, use 'venv\Scripts\activate'
```
## 3. Install Dependencies
Run the following command to install all the required dependencies:
```
pip install streamlit boto3 pyaudio SpeechRecognition
```

## 4. Setting Up AWS Credentials
To access AWS Polly, you need to provide your AWS credentials. These can be hardcoded in the script or configured through environment variables. If using temporary credentials, include `AWS_SESSION_TOKEN` as shown in the script.

### Example of setting environment variables in Linux/macOS:
```
export AWS_DEFAULT_REGION="us-west-2"
export AWS_ACCESS_KEY_ID="YOUR_ACCESS_KEY_ID"
export AWS_SECRET_ACCESS_KEY="YOUR_SECRET_ACCESS_KEY"
export AWS_SESSION_TOKEN="YOUR_SESSION_TOKEN"  # If using temporary credentials
```
## 5. Running the Application
To start AccentFlow, navigate to the root directory of the project and run the following command:
```
streamlit run streamlit_app.py
```

## Troubleshooting Audio Issues
### For Linux Users:
If you are facing issues with PyAudio, make sure you have `portaudio` installed:
```
sudo apt-get install portaudio19-dev
```

### For macOS Users:
Install PyAudio dependencies using Homebrew:
```
brew install portaudio
pip install pyaudio
```


