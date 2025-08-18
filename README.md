# Video-OCR-Extraction
Extract text from video frames using Tesseract OCR and OpenCV


# 🎥 Video OCR Text Extraction

This project extracts text from video frames using **OpenCV** and **Tesseract OCR**.  
The script processes a video file frame by frame, applies preprocessing (grayscale + thresholding), and saves all extracted text to a file.

---

## 📂 Project Structure
video-ocr-extraction/
│── main.py # Main script (your code)
│── requirements.txt # Python dependencies
│── README.md # Project documentation
│── output/ # Folder where extracted text is saved

yaml
Copy
Edit

---

## ⚙️ Installation

1. **Clone the repository**
```bash
git clone https://github.com/your-username/video-ocr-extraction.git
cd video-ocr-extraction
Install dependencies

bash
Copy
Edit
pip install -r requirements.txt
Install Tesseract OCR (Linux / Kaggle / Colab)

bash
Copy
Edit
sudo apt-get update
sudo apt-get install -y tesseract-ocr
The script already points to the correct path for Linux:

python
Copy
Edit
pytesseract.pytesseract.tesseract_cmd = r'/usr/bin/tesseract'
▶️ Usage
Place your video in the input directory and update the path in main.py:

python
Copy
Edit
video_path = '/kaggle/input/ai-video/ai video.mp4'
Run the script:

bash
Copy
Edit
python main.py
📂 Output
Extracted text is saved in:

bash
Copy
Edit
output/extracted_text.txt
