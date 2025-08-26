# **🎙️ MagicTypes: Voice-to-Text Transcription Suite**

MagicTypes is a sophisticated voice recording and transcription toolkit that leverages OpenAI's Whisper for accurate speech-to-text conversion. It features a comprehensive dashboard for managing transcription history, exception-based text replacement, and real-time monitoring capabilities.

---

## 🛠️ Core Components

### 🎙️ Voice Recorder & Transcriber
- Record audio via microphone using global hotkeys (Shift+Alt+W)
- Transcribe recordings using Whisper's small model (CPU-only)
- Automatic copying of transcribed text to clipboard
- Audio feedback with configurable beep notifications

### 📝 Exception-Based Text Replacement
- Define custom text replacement rules in Exception.txt
- Case-insensitive matching with word boundary support
- Real-time rule reloading when files change
- Web-based rule editor with live preview

### 📊 History Dashboard
- Web interface showing all transcription history
- Words-per-minute (WPM) calculations and statistics
- Monthly history files with detailed timestamps
- Copy functionality for previous transcriptions

### 🔧 Rule Editor
- Dedicated web interface for managing replacement rules
- Add/delete rules without restarting the main application
- Real-time synchronization with main application

---

## ⚙️ Technical Architecture

- **Flask Backend** (`c.py`/`MagicTypes Main Code.py`)
  - Dual server architecture (main app + editor)
  - REST API endpoints for all functionality
  - Server-Sent Events (SSE) for real-time updates

- **Audio Processing**
  - 16kHz sample rate recording via sounddevice
  - Temporary WAV file creation and cleanup
  - Thread-safe recording operations

- **Text Processing**
  - Whisper model running on CPU with configurable threads
  - Sophisticated pattern matching for text replacement
  - Case normalization and word boundary detection

- **File Monitoring**
  - Watchdog-based monitoring of history and exception files
  - Automatic reloading of rules when Exception.txt changes
  - Real-time dashboard updates when new history is created

---

## ✨ Key Features

- **Hotkey Controls**: Global keyboard shortcuts for recording/quit
- **Real-time Updates**: Live dashboard updates via SSE
- **Dark/Light Mode**: Theme switching with persistent preferences
- **Export Ready**: All transcriptions saved in parseable text format
- **Privacy Focused**: Everything runs locally on your machine
- **Performance Optimized**: Configurable CPU core usage

---

## 🧭 Getting Started

1. **Install dependencies**:
   ```bash
   pip install sounddevice whisper pyperclip keyboard torch numpy scipy winsound flask requests watchdog
   ```

2. **Run the application**:
   ```bash
   python "MagicTypes Main Code.py"
   ```

3. **Access the dashboard**:
   - Automatically opens at http://127.0.0.1:5000/
   - Or manually navigate to the shown URL

4. **Using the tool**:
   - Press `Shift+Alt+W` to start/stop recording
   - Press `Shift+Alt+Q` to quit the application
   - Use the dashboard to view history and edit exception rules

---

MagicTypes brings professional-grade voice transcription to your local machine with privacy-focused processing and powerful text replacement capabilities - perfect for journalists, developers, students, and anyone who needs accurate speech-to-text conversion.

---

## 🤖 Bonus

Yes, parts of this were co-developed with AI - because sometimes you need a virtual assistant to build a virtual assistant.

---

## 📜 License

This document is licensed under  
**[CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/)**  
> You can use the tool, you can marvel at its capabilities, but you can't resell or remix this documentation without permission.

---

*Note: The system uses OpenAI's Whisper model under the hood, but all processing happens locally on your machine - no data is sent to external servers.*
