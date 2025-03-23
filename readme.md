
### 📄 `README.md`

```markdown
# Hebrew PDF to Word Converter 📝🇮🇱

A Python tool to convert Hebrew-language PDF files (including scanned images) into fully formatted Word (`.docx`) documents using OCR (Optical Character Recognition). Designed to preserve Hebrew text direction, formatting, and layout — perfect for legal or official documents.

---

## ✨ Features

- ✅ Supports scanned PDFs using Tesseract OCR
- 🕍 Right-to-left (RTL) paragraph formatting for Hebrew
- 🔤 Uses a Hebrew-compatible font (`David`)
- 📄 Automatically adds bold headers for legal keywords
- 🧠 Groups OCR words into real lines to preserve layout
- 🖼️ Enhances image quality for better OCR accuracy
- 📑 Page breaks added between PDF pages

---

## 📦 Requirements

Make sure you have the following installed:

```bash
sudo apt install tesseract-ocr libtesseract-dev poppler-utils
pip install pytesseract pdf2image python-docx pillow
```

You’ll also need the Hebrew Tesseract language pack:

```bash
sudo apt install tesseract-ocr-heb
```

---

## 🚀 Usage

Run the converter script:

```bash
python pdf_to_word.py
```

1. A file dialog will pop up.
2. Choose a Hebrew PDF (scanned or text-based).
3. The script will process each page and create a `.docx` file next to the original PDF.

---

## 📁 Output

The generated Word file will:
- Have the same page structure as the original
- Contain readable and selectable Hebrew text
- Use appropriate formatting for titles and body text

Example output file:
```
your_file.pdf → your_file_formatted.docx
```

---

## 🧪 Tips for Better OCR

- Use high-quality scanned PDFs (300 DPI recommended)
- If text is missing, try increasing contrast or rescanning
- Works best with documents that have typed text (not handwriting)

---

## 🛠️ File Structure

```
convert_img_word/
│
├── pdf_to_word.py       # Main OCR script
├── README.md            # This file
```

---

## 🧑‍💻 Author

Developed by [Your Name] – Feel free to contribute or suggest improvements!

---

