# 📷🗣️ Text Reader & Voice Assistant

A real-time, camera-powered text reader with multilingual OCR and voice playback. Bring text on paper or screens to life using your webcam! Supports English 🇬🇧, Bengali 🇧🇩, Hindi 🇮🇳, and Tamil 🇮🇳.

---

## 🚀 Features

- 🎥 **Live Camera Preview** with enhanced GUI overlay  
- 👁️‍🗨️ **Instant OCR** from a smart capture area  
- 🔊 **Text-to-Speech** for extracted text  
- 🌐 **Multiple Languages:** English, Bengali, Hindi, Tamil (press 1–4)  
- ⌨️ **Hotkey Controls:**  
  1️⃣ 2️⃣ 3️⃣ 4️⃣ — Change language  
  ⬜ **SPACE** — Capture & Read Text  
  🔁 **R** — Repeat Last Text  
  ❌ **Q** — Quit Application  
- 🪞 **Mirror Mode** for easy point-and-capture interface  

---

## 🏁 Getting Started

### 1️⃣ Prerequisites

- Python 3.7+  
- [Tesseract OCR](https://github.com/tesseract-ocr/tesseract) installed and added to your system PATH  

### 2️⃣ Installation
-git clone https://github.com/rivu-intel45/luna-reader.git 
-pip install -r requirements.txt
### 3️⃣ Tesseract Setup

- 🪟 **Windows**: [Download installer](https://github.com/tesseract-ocr/tesseract) and complete setup  
- 🐧 **Linux**:  sudo apt-get install tesseract-ocr tesseract-ocr-ben tesseract-ocr-hin tesseract-ocr-tam
- 🍏 **macOS**:  brew install tesseract
For full language support, make sure `ben.traineddata`, `hin.traineddata`, and `tam.traineddata` are present in your `tessdata` folder.

---

## ⚡ Usage

Update the Tesseract path in your code if needed:
pytesseract.pytesseract.tesseract_cmd = r"C:\Program Files\Tesseract-OCR\tesseract.exe"

Then start the notebook or script and point your camera at the text inside the green capture box.

---

## 🎛️ Controls

| Key   | Action                    | Emoji |
|-------|---------------------------|-------|
| 1     | Switch to English         | 🇬🇧   |
| 2     | Switch to Bengali         | 🇧🇩   |
| 3     | Switch to Hindi           | 🇮🇳   |
| 4     | Switch to Tamil           | 🇮🇳   |
| SPACE | Capture & Read Text       | ⬜️    |
| R     | Repeat Last Text          | 🔁    |
| Q     | Quit Application          | ❌    |

---

## 📦 Dependencies

- opencv-python  
- pytesseract  
- pillow  
- gtts  
- pygame  
- numpy  

Install everything with:
-pip install -r requirements.txt
---

## 💡 Troubleshooting

- ⚠️ **Tesseract not found?** Check the `tesseract_cmd` path and PATH configuration.  
- 🔇 **No audio?** Verify system volume, default output device, and `pygame` installation.  
- 📋 **No text detected?** Improve lighting, adjust focus, and keep text fully inside the capture box.  

---

## 🙌 Contributing

Pull requests are welcome!  
For major changes, please open an issue first to discuss what you would like to improve or add.
