# Manga Text Extractor v1.0

Simple Python tool to extract English text from manga pages using EasyOCR with visual bounding boxes.

## 📦 Installation

### 1. Clone the repository
```bash
git clone https://github.com/danieln0bre/op_reader.git
cd op_reader
```

### 2. Setup virtual environment

```bash
python -m venv venv
source venv/bin/activate  # Linux/Mac
.\venv\Scripts\activate  # Windows
```

### 3. Install requirements

```bash
pip install easyocr opencv-python matplotlib numpy
```
### 🛠️ Usage

 Add your manga page as TEST.jpeg to the project folder.
 Run the extractor.

### ⚙️ Configuration Tips
Adjust in manga_extractor:
```bash
reader.readtext(image_path,
              text_threshold=0.7,  # 0-1 (higher = more strict)
              low_text=0.4,        # 0-1 (lower = better for small text)
              mag_ratio=1.5)       # 1.0-2.0 (zoom factor)
``` 
