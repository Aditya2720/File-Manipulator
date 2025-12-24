# File-Manipulator
Offline File Manipulator is a lightweight desktop app for converting, compressing, and extracting files fully offline. It supports images, PDFs, and Excel files with tools like image to PDF, PDF to image or Excel, image compression, and OCR. All processing happens locally with no uploads, tracking, or internet use, ensuring complete privacy.
# ◆ File Converter Pro

**Professional-grade file conversion and compression** — completely offline, completely private.

![License](https://img.shields.io/badge/License-MIT-1a1a1a?style=flat-square&logo=github)
![Python](https://img.shields.io/badge/Python-3.10+-00d9ff?style=flat-square)
![Status](https://img.shields.io/badge/Status-Production%20Ready-00ff41?style=flat-square)
![Theme](https://img.shields.io/badge/Theme-Premium%20Black-0f0f0f?style=flat-square)

---

## ⚡ 30-Second Setup

```bash
cd file_manipulator
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
python app.py
```

**That's it.** Your app is ready.

---

## 🎯 What This Does

Convert and compress **any file type** with a premium, intuitive interface. 
- ✅ **100% Offline** — No cloud, no tracking
- ✅ **Simple Interface** — Drag & drop, click convert
- ✅ **Batch Processing** — Handle multiple files at once
- ✅ **Quality Control** — Low/Medium/High options
- ✅ **Real-time Progress** — Watch conversions happen

---

## 📋 Requirements

| Item | Version |
|------|---------|
| **Python** | 3.10+ |
| **Windows** | 7+ (10+ recommended) |
| **RAM** | 2+ GB |
| **Disk** | 500 MB |

### Optional Dependencies
- **LibreOffice** — For Excel/PowerPoint conversions
- **Tesseract** — For image-to-text OCR
- **ImageMagick** — For advanced image operations

---

## ✨ Conversion Types

### Always Available
- **Image → PDF** — JPG, PNG, WebP to PDF
- **Image Compression** — Reduce size with quality control
- **Image Format** — JPG ↔ PNG ↔ JPEG conversions
- **PDF → Images** — Extract pages as JPEGs (72-200 DPI)
- **PDF → Long Image** — Stack all pages vertically
- **PDF Compression** — Intelligently reduce file size
- **Any File → ZIP** — Archive with compression

### With LibreOffice
- **Excel → PDF** — Spreadsheet conversion
- **Excel → Image** — Generate previews
- **PowerPoint → PDF** — Presentation export

### With Tesseract
- **Image → Text** — OCR text extraction

### Advanced
- **PDF → Excel** — Extract tables and data
- **Batch Operations** — Process 100+ files at once

---

## 🎨 Design Features

### Premium Interface
- **Dark Theme** — Easy on the eyes, professional appearance
- **Cyan Accents** — Modern, elegant visual hierarchy
- **Real-time Feedback** — Status indicators and progress tracking
- **Emoji Icons** — Intuitive action buttons
- **Flat Design** — Clean, minimal, sophisticated

### User Experience
- **Drag & Drop** — Add files instantly
- **Auto-Detection** — Recognizes file types automatically
- **Smart Defaults** — Conversion type pre-selected
- **History Sidebar** — Track last 20 conversions
- **One-Click Output** — Open results folder instantly

---

## 📁 Project Structure

```
file_manipulator/
├── app.py                    # Main application (redesigned UI)
├── requirements.txt          # Dependencies
│
├── core/
│   ├── dispatcher.py        # Conversion router
│   └── file_detector.py     # File type detection
│
├── converters/
│   ├── image_to_pdf.py      # Image → PDF
│   ├── pdf_to_image.py      # PDF → Image
│   ├── pdf_to_excel.py      # PDF → Excel
│   ├── excel_to_pdf.py      # Excel → PDF
│   ├── ppt_to_pdf.py        # PPT → PDF
│   └── zip_file.py          # Compression
│
├── compressors/
│   ├── image_compress.py    # Image optimization
│   └── pdf_compress.py      # PDF optimization
│
├── ocr/
│   └── image_to_text.py     # OCR engine
│
├── utils/
│   ├── paths.py             # Path utilities
│   └── validators.py        # Input validation
│
├── output/                  # Results directory
└── setup/                   # Documentation
```

---

## 🚀 Quick Start

### 1️⃣ Installation

**Windows 10+:**
```bash
# Clone/download the project
cd file_manipulator

# Create virtual environment
python -m venv .venv

# Activate it
.venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run
python app.py
```

### 2️⃣ Basic Usage

1. **Add Files** — Drag & drop or click "Add Files"
2. **Select Action** — Auto-selected based on file type
3. **Choose Quality** — Low/Medium/High (if applicable)
4. **Click START** — Conversion begins
5. **Check Output** — Results in output folder

### 3️⃣ Optional Enhancements

For advanced features, install optional tools:

```bash
# Excel/PowerPoint support
# Download: https://www.libreoffice.org/download/

# Image OCR support
# Download: https://github.com/UB-Mannheim/tesseract/wiki
```

---

## 💡 Common Tasks

### Compress an Image
1. Add image file
2. Select "image_compress"
3. Choose quality: **High**
4. Click START

### Convert PDF to Images
1. Add PDF file
2. Auto-selects "pdf_to_image"
3. Choose quality: **High** (200 DPI)
4. Click START

### Extract Text from Image
1. Add image file (requires Tesseract)
2. Select "image_to_text"
3. Click START

### Archive Multiple Files
1. Add 3+ files
2. Select "zip_file"
3. Choose compression: **High**
4. Click START

---

## 🔐 Privacy & Security

```
✅ 100% Offline         — No internet connection required
✅ No Cloud Upload      — All processing is local
✅ No Telemetry        — Zero tracking or data collection
✅ Open Source         — Full code transparency
✅ No Admin Rights     — Runs as regular user
✅ No Data Collection  — Files never leave your computer
```

---

## ⚙️ System Requirements

**Minimum Configuration:**
- Windows 7 or later
- Python 3.10+
- 2 GB RAM
- 500 MB disk space

**Recommended Configuration:**
- Windows 10+ or Windows 11
- Python 3.11+
- 4+ GB RAM
- 1+ GB disk space

**Supported Platforms:**
- ✅ Windows 7, 8, 10, 11
- ✅ Python 3.10, 3.11, 3.12

---

## 🛠️ Configuration

### Set Output Folder
Click "Output Folder" button to choose where files are saved.

### Quality Levels
- **Low** — Smaller files, lower quality (good for web)
- **Medium** — Balanced (recommended)
- **High** — Best quality, larger files

### Batch Processing
Add multiple files at once. The app processes them sequentially with progress tracking.

---

## 🐛 Troubleshooting

### Python not found?
```bash
python --version
```
If this fails, reinstall Python from https://www.python.org with "Add to PATH" checked.

### Module not found?
```bash
.venv\Scripts\activate
pip install -r requirements.txt --upgrade
```

### LibreOffice not detected?
Ensure LibreOffice is installed in the default location:
```
C:\Program Files\LibreOffice
```

### Tesseract not working?
Install from: https://github.com/UB-Mannheim/tesseract/wiki

### Performance issues?
- Close other applications
- Reduce quality level to "Low"
- Process fewer files at once

For more help, see [setup/TROUBLESHOOTING.md](setup/TROUBLESHOOTING.md).

---

## 📚 Documentation

| Document | Purpose |
|----------|---------|
| [setup/SETUP.md](setup/SETUP.md) | Detailed installation guide |
| [setup/USAGE.md](setup/USAGE.md) | Feature documentation |
| [setup/TROUBLESHOOTING.md](setup/TROUBLESHOOTING.md) | Common issues & solutions |
| [setup/OPTIONAL_TOOLS.md](setup/OPTIONAL_TOOLS.md) | Optional dependencies |

---

## 🎨 Interface Highlights

### Header
- **Status Indicator** — Real-time conversion status (Ready/Converting/Complete)
- **Title Bar** — Clean, professional appearance
- **Dynamic Feedback** — Color-coded status (green/amber/red)

### Sidebar
- **Quick Actions** — Add files, folders, manage output
- **Queue Status** — See how many files are ready
- **Conversion History** — Last 20 conversions with status (✓/✗)
- **Output Directory** — Current save location

### Main Interface
- **Drag & Drop Zone** — Large, prominent drop area
- **File Queue** — Shows all files ready for conversion
- **Settings Panel** — Choose conversion type and quality
- **Progress Bar** — Real-time conversion progress
- **Status Log** — Detailed conversion messages

---

## 📊 Features at a Glance

| Feature | Support |
|---------|---------|
| Drag & Drop | ✅ Full support |
| Batch Processing | ✅ Unlimited files |
| Quality Control | ✅ Low/Medium/High |
| Progress Tracking | ✅ Real-time |
| Conversion History | ✅ Last 20 items |
| Dark Theme | ✅ Included |
| Offline Mode | ✅ 100% offline |
| Auto File Detection | ✅ Automatic |
| Output Folder | ✅ Customizable |

---

## 🔄 How It Works

1. **File Detection** — App identifies file type automatically
2. **Action Selection** — Suggests appropriate conversions
3. **Quality Selection** — Choose output quality (if applicable)
4. **Batch Processing** — Handles multiple files
5. **Real-time Progress** — See each file being converted
6. **Status Feedback** — Success/error for each file
7. **Auto Save** — Results saved to output folder
8. **History Tracking** — Last 20 conversions logged

---

## 💼 Professional Use Cases

- **Marketing Teams** — Convert images and PDFs for campaigns
- **Content Creators** — Optimize images and documents
- **Business Users** — Convert Excel/PowerPoint offline
- **Developers** — Batch process file formats
- **Privacy-Conscious Users** — 100% local processing
- **Offline Workers** — No internet connection needed

---

## 📝 Version Info

**Latest Version:** 2.0 (Design Update)  
**Release Date:** December 24, 2025  
**Status:** ✅ Production Ready  
**License:** MIT (Open Source)

---

## 🎉 Get Started

```bash
cd file_manipulator
python app.py
```

**Convert anything. Offline. Professionally.**

---

## 📞 Support

- Check [setup/TROUBLESHOOTING.md](setup/TROUBLESHOOTING.md) for common issues
- Review [setup/USAGE.md](setup/USAGE.md) for detailed feature guides
- See [setup/OPTIONAL_TOOLS.md](setup/OPTIONAL_TOOLS.md) for advanced setup

**Questions?** All documentation is included in the `/setup/` folder.

---

**Made with ◆ • 100% Offline • 100% Private • Production Ready**

