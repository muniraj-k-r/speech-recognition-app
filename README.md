# 🗣️ Speech Recognition Library

A robust and modular Python library for speech recognition using microphone or audio files. Supports multiple speech engines (e.g., Google Web Speech API, Microsoft Azure, Amazon Transcribe), works offline with FLAC conversion, and handles real-time or recorded audio.

---

## 📦 Features

- 🎤 Recognize speech via **microphone** or **WAV/AIFF/FLAC** audio files
- 🌐 API support: **Google**, **Azure**, **Amazon**, **Wit.ai**, **Houndify**, and **Lex**
- 🔇 Automatic adjustment to ambient noise
- 📁 Includes platform-specific FLAC binaries for **Windows**, **macOS**, and **Linux**
- 📚 Modular Python package with clean OOP design and exception handling
- ⚡ Simple `__main__.py` script to test microphone input quickly

---

## 🚀 Getting Started

### 🔧 Installation

1. Clone the repository:

```bash
git clone https://github.com/muniraj-k-r/speech-recognition-app.git
cd speech-recognition-app
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

> 🔸 If `pyaudio` installation fails, try:
```bash
pip install pipwin
pipwin install pyaudio
```

---

## 🛠️ Project Structure

```
speech_recognition_app/
├── speech_recognition/
│   ├── __init__.py
│   ├── __main__.py
│   ├── audio.py
│   ├── exceptions.py
│   ├── flac-win32.exe
│   ├── flac-mac
│   ├── flac-linux-x86
│   └── flac-linux-x86_64
├── requirements.txt
├── LICENSE
└── README.md
```

---

## 🧪 Usage

### 🖥️ Run Demo (via Microphone)

```bash
python -m speech_recognition
```

Sample output:

```
A moment of silence, please...
Set minimum energy threshold to 400
Say something!
Got it! Now to recognize it...
You said: hello world
```

---

### 🗃️ Use with Audio Files

```python
from speech_recognition.audio import AudioData
audio = AudioData.from_file("sample.wav")
print(audio.get_wav_data())
```

---

## 📤 API Support

Integrate with cloud APIs using:
- `recognize_google()`
- `recognize_azure()`
- `recognize_amazon()`
- `recognize_wit()`
- `recognize_houndify()`
- `recognize_lex()`

---

## 📜 License

Licensed under the **BSD License**. See [LICENSE](LICENSE) file.

---

## 🤝 Contributing

We welcome pull requests and feedback!

---

## 🙋 Author

**Muniraja K R**  
GitHub: [@muniraj-k-r](https://github.com/muniraj-k-r)
