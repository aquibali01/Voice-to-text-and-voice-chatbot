# Voice-to-Voice Chatbot using Whisper, LLaMA, and Groq API

This project is a real-time voice-to-voice chatbot that leverages OpenAI's Whisper for speech-to-text transcription, LLaMA 8B via the Groq API for generating responses, and Google Text-to-Speech (gTTS) for converting text back into speech. The chatbot interface is built using Gradio, allowing users to interact with the bot by speaking or uploading audio files.

## Features

- **Speech-to-Text**: Convert spoken language into text using OpenAI's Whisper model.
- **AI-Generated Responses**: Use LLaMA 8B via the Groq API to generate intelligent responses based on the transcribed text.
- **Text-to-Speech**: Convert the generated text responses back into speech using Google Text-to-Speech (gTTS).
- **Real-Time Interaction**: The chatbot works in real-time, allowing users to interact through a microphone or by uploading audio files via a web interface.
  
## Prerequisites

Before you begin, ensure you have met the following requirements:

- Python 3.7 or higher installed on your local machine or Google Colab.
- A Groq API key. You can sign up for an API key [here](https://groq.com/).
- [Google Colab](https://colab.research.google.com/) or a local Python environment with necessary libraries installed.

## Installation

Follow these steps to set up the project:

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/your-username/voice-to-voice-chatbot.git
   cd voice-to-voice-chatbot

**Install Dependencies:**

Install the required Python libraries:

   ```bash
   pip install -r requirements.txt



Alternatively, if you are using Google Colab, you can install the libraries using:


  ```bash
  !pip install gradio groq-api openai-whisper gtts

Set Up Groq API Key:

Add your Groq API key to the environment variables:

  ```bash
  export GROQ_API_KEY='your_groq_api_key'

In Google Colab, you can set the API key using:

  ```python
  import os
  os.environ['GROQ_API_KEY'] = 'your_groq_api_key'

Usage
To start the chatbot, run the main script:

  ```python
  python app.py

Or in Google Colab:

Copy the script to a code cell and execute.

The Gradio interface will launch, allowing you to interact with the chatbot.
Interacting with the Chatbot

Using Microphone: Speak directly into the microphone. The chatbot will transcribe your speech, generate a response, and play it back as audio.

Uploading Audio: Upload a pre-recorded audio file. The chatbot will transcribe the audio, generate a response, and convert the response back to speech.

Project Structure

  ```bash
  voice-to-voice-chatbot/
  ├── app.py                 # Main script to run the chatbot
  ├── requirements.txt       # List of Python dependencies
  ├── README.md              # Project documentation
  └── .gitignore             # Git ignore file

Troubleshooting

Common Issues

ModuleNotFoundError: Ensure you have installed the correct version of the Whisper module with !pip install -U openai-whisper

Groq API Key Error: Double-check your API key and ensure it is set in the environment variables correctly.
Logging and Debugging


Contributing

Contributions are welcome! Please fork this repository, create a new branch, and submit a pull request with your changes.

License
This project is licensed under the MIT License. See the LICENSE file for details.
