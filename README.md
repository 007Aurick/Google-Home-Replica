🎙️ Voice Assistant with Speech Recognition & TTS

A simple voice-controlled assistant built using Google Cloud Speech-to-Text and Text-to-Speech APIs, capable of listening to user commands and responding with audio in real time.

📌 Features
🎤 Records user voice input
🧠 Converts speech → text using Google Speech-to-Text
🔊 Responds using Text-to-Speech
🪙 Flip a coin (heads/tails)
📅 Tells today’s date
➕ Performs basic math ( +, −, ×, ÷ )
🎵 Plays music on command
🔁 Runs in a continuous voice loop
🧠 How It Works
The assistant asks: “What do you want?”
Records audio for 5 seconds
Converts speech → text using Google Cloud
Parses the command
Executes action (calculation, date, etc.)
Responds using generated speech
🛠️ Tech Stack
Python
Google Cloud Speech-to-Text
Google Cloud Text-to-Speech
SoundDevice (audio recording)
SoundFile + SciPy
OS / subprocess
⚙️ Setup
1. Install dependencies
pip install google-cloud-speech google-cloud-texttospeech sounddevice soundfile scipy
2. Google Cloud Setup
Create a Google Cloud project
Enable:
Speech-to-Text API
Text-to-Speech API
Download your service account JSON key
Replace:
'vision-project-207707-f84d39ceed76.json'

with your own credentials file

▶️ Usage

Run the script:

python main.py(or whatever your filing naming convention is)

The assistant will continuously listen and respond.

🎤 Supported Commands
Command	Action
“flip a coin”	Returns heads or tails
“today’s date”	Speaks current date
“3 + 5”	Performs calculation
“play a song”	Plays music file
“stop”	Ends program

⚠️ Limitations
Fixed 5-second recording window
Limited natural language understanding
Requires internet (Google APIs)
Hardcoded credentials path (needs improvement)

🔮 Future Improvements
Wake word detection (like “Hey Assistant”)
Continuous streaming (no fixed recording window)
NLP for better command parsing
Integration with smart devices / IoT
Bluetooth speaker output
Edge deployment (offline version)

👤 Author

Built as a voice interface project combining AI APIs + real-time audio processing.
