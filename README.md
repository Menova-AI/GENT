
# GENT (GUI Element Navigation Tool)

[Watch the video!](https://www.youtube.com/embed/ujHkVyDFQq4?si=wATyUDwomrSl7WXb)

GENT is an advanced desktop automation tool that combines computer vision, natural language processing, and mouse/keyboard control to enable intuitive, voice-controlled interaction with any graphical user interface.

## 🌟 Key Features

- **Natural Language Control**: Control your computer using plain English voice commands
- **Computer Vision Integration**: Automatically detects and classifies GUI elements like buttons, fields, links, and images
- **Intelligent Navigation**: Smart element targeting and navigation based on visual context
- **Voice Recording**: Built-in audio processing for voice command input
- **Multi-Monitor Support**: Works across multiple displays with primary monitor detection
- **Adaptive Screenshots**: Takes and analyzes screenshots only when significant changes occur
- **Smart Element Selection**: Supports various mouse actions including click, right-click, double-click, drag-and-drop
- **Audio Feedback**: Provides audio confirmation for successful command processing

## 🚀 Getting Started

### Prerequisites

```bash
# Required Python packages
pip install pyaudio wave numpy pydub openai pillow opencv-python easyocr torch ultralytics screeninfo pyautogui
```

### Environment Setup

1. Create a `.env` file with your OpenAI API key:
```
OPENAI_API_KEY=your_api_key_here
```

2. Install Flameshot for screenshot functionality:
```bash
# Ubuntu/Debian
sudo apt-get install flameshot

# Fedora
sudo dnf install flameshot

# Arch Linux
sudo pacman -S flameshot
```

## 💡 Usage

### Basic Commands

GENT supports a wide range of natural language commands:

- **Click Operations**: 
  - "click here"
  - "right click on [element]"
  - "double click on [element]"
  
- **Text Operations**:
  - "write [text] here"
  - "copy [element]"
  - "paste here"
  
- **Navigation**:
  - "move to [position]"
  - "scroll up/down"
  - "next element right/left/up/down"
  
- **Selection**:
  - "select [elements]"
  - "drag from here to [element]"

### Advanced Features

- **Intelligent Element Finding**: GENT uses computer vision to identify GUI elements and their locations
- **Context-Aware Actions**: Commands are interpreted based on the current screen context
- **Multi-Step Operations**: Supports complex sequences of actions
- **Adaptive Screenshot Analysis**: Only processes new screenshots when significant changes occur

## 🔧 Technical Details

### Screenshot Processing

- Uses Flameshot for high-quality screen capture
- Implements difference detection to minimize unnecessary processing
- Supports multi-monitor configurations

### Element Detection

- Classifies GUI elements into categories:
  - Buttons
  - Images
  - Links
  - Text

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

[If you want to support the efforts of Menova AI, consider joining our patreon so we can continue making AI accessible to everyone.](https://www.patreon.com/c/MenovaAI)

## 📝 License

This project is licensed under the AGPL-3.0 license - see the LICENSE file for details.

## ⚠️ Disclaimer

This tool is designed for legitimate automation purposes. Users are responsible for ensuring compliance with relevant policies and regulations when using this tool.
