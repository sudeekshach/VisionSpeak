# 🧠 VisionSpeak: Hands-Free OCR & Text-to-Speech Assistant

> An assistive tool that reads printed text aloud for the visually impaired using real-time OCR and speech synthesis. Just point your camera — no clicks needed.

---

## 📸 What It Does

- ✅ Automatically detects and corrects **page orientation** (even if upside down)
- ✅ Reads **printed English text aloud** using Google's Text-to-Speech (gTTS)
- ✅ Provides **voice-based instructions** if the page is too far, small, or misaligned
- ✅ Works in real-time using webcam and OpenCV
- ✅ Completely **hands-free** — no buttons, no input required

---

## 🔧 How It Works

1. Captures webcam input every 5 seconds
2. Automatically detects page tilt or upside-down orientation
3. Uses Tesseract OCR to extract text from the frame
4. Compares the result with previous text to avoid repetition
5. Speaks the newly detected text using gTTS
6. Guides the user to adjust the page if no readable text is found

---

## 🛠️ Requirements

- Python 3.7 or newer
- [Tesseract OCR](https://github.com/UB-Mannheim/tesseract/wiki) (Windows: install and add to PATH)
- Install Python packages with:

```bash
pip install opencv-python pytesseract gTTS playsound==1.2.2
