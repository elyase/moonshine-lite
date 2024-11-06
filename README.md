# 🎙️ Moonshine Lite

> 🚀 A lightweight Python wrapper for the [moonshine](https://github.com/usefulsensors/moonshine/) speech-to-text models with real-time transcription capabilities

## ✨ Features

- ⚡ Small and fast (60MB model size)
- 🎤 Real-time transcription from microphone
- ⌨️ Simulated keyboard typing for app integration
- 📝 Support for WAV file transcription
- 🎯 Simple API (`listen` and `transcribe` methods)

## 🚀 Quick Start

### Installation

```bash
pip install moonshine-lite
```

### Basic Usage

```python
from moonshine_lite import Moonshine

moonshine = Moonshine()

# Transcribe a WAV file
text = moonshine.transcribe("audio.wav")
print(text)

# Start live transcription (text will be typed in the current application)
# you need to press and hold the activation key (Cmd by default) to start listening
moonshine.listen()
```

### 💻 CLI

```bash
# Transcribe a WAV file
moonshine transcribe "audio.wav"

# Start live transcription (text will be typed in the current application)
# you need to press and hold the activation key (Cmd by default) to start listening
moonshine listen

# Use tiny model
moonshine --model moonshine/tiny listen
```

## 🙏 Credits

- [Useful Sensors' Moonshine models](https://github.com/usefulsensors/moonshine/)
- [Silero VAD](https://github.com/snakers4/silero-vad) for voice activity detection

## 📚 Documentation

No need :-D

---

Made with ❤️ by [Yaser Martinez Palenzuela](https://github.com/elyase)
