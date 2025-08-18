# 🎥 Video OCR Text Extraction

This project extracts text from video frames using **OpenCV** and **Tesseract OCR**.  
The script processes a video file frame by frame, applies preprocessing (grayscale + thresholding) and saves all extracted text to a file.



## ⚙️ Installation

1. **Clone the repository**
```bash
git clone https://github.com/Abdullah012472/Video-OCR-Extraction.git
```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Install Tesseract OCR (Linux / Kaggle / Colab)**
   ```bash
   sudo apt-get update
   sudo apt-get install -y tesseract-ocr
   ```
The script already points to the correct path for Linux:
```bash
pytesseract.pytesseract.tesseract_cmd = r'/usr/bin/tesseract'
```
## ▶️ Usage
1. Place your video in the input directory and update the path in main.py:
```bash
video_path = '/kaggle/input/ai-video/ai video.mp4'
```
2. Run the file:
```bash
python main.py
```
📂 Output
Extracted text is saved in:

output/extracted_text.txt
