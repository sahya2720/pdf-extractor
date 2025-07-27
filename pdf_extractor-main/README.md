
# 🧾 PDF_Extractor

This project is a Python tool that automatically extracts an outline structured  from PDF documents by considering the visual layout and format of the text. It identifies the main titles, such as the title, H1, H2 and H3, based on the size and style of the font, and creating a clear and decentralized JSON structure. This tool operates completely offline, helping it fit the safe environment and is designed to quickly handle large PDF files. It is perfect for tasks such as summarizing documents, smart research and creating dynamic content tables.
## 📦 Features
🌐 Multilingual Heading Detection
Supports documents written in English, Hindi, Japanese, and other Unicode-based languages — ideal for global users and diverse datasets.

🚀 Fast & Lightweight
Uses PyMuPDF for high-speed parsing without relying on large machine learning models — processes 50-page PDFs in seconds.

🧠 Smart Visual Hierarchy Recognition
Identifies headings like Title, H1, H2, and H3 based on font size, style, and layout — works even on untagged or scanned PDFs with text layers.

🔒 Offline & Privacy-Preserving
Runs entirely on your local machine — no cloud, no API keys, no data leakage.

🐳 Easy to Deploy Anywhere
Comes with a ready-to-use Docker container — one command to run on any platform or environment.
## 🛠 Requirements
Python 3.8+

pip

Dependencies:

```bash
  pip install -r requirements.txt
```
Or

install manually:

```bash
  pip install PyMuPDF
```

## 🧪 How to Use
Run from command line

```bash
python extract_outline.py yourfile.pdf
```

This will print the outline structure in your terminal.

Sample Output:

```json

{
  "title": "Sample PDF Title",
  "headings": [
    {
      "level": "H1",
      "text": "Introduction"
    },
    {
      "level": "H2",
      "text": "Background"
    },
    ...
  ]
}
```
## 📁 File Structure

```
pdf_extractor/
├── input/ → Folder for input PDFs
│ └── sample.pdf → (Example PDF file)
│
├── output/ → Output JSON files saved here
│ └── sample.json → (Example output outline)
│
├── main.py → Main script to run PDF outline extraction
├── heading_extractor.py → Core logic to extract headings from a PDF
├── utils.py → (Optional) Helper functions (e.g., for multilingual processing)
├── requirements.txt → List of Python dependencies (e.g., PyMuPDF)
├── Dockerfile → Docker setup for containerized execution
├── README.md → Project description, setup, usage, features
├── LICENSE → (Optional) License file (MIT recommended)
└── .gitignore → Ignores venv, pycache, etc.
```
## 👩‍💻 Authors

- [@octokatherine](https://www.github.com/octokatherine)

