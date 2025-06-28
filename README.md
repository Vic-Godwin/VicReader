# VicReader
VicReader is an efficient, self-contained analysis tool for only .txt files — perfect for students, writers, developers, and data workers who work with structured or unstructured text.

# 📖 VicReader

![image](https://github.com/user-attachments/assets/01086612-166d-4d11-8acb-fa01eb7763b4)


**Smart, Searchable File Reader & Text Extractor Companion for [VictorCompress](https://github.com/Vic-Godwin/VictorCompress)**

VicReader is a lightweight but powerful file analysis and viewer tool that works alongside [VictorCompress](https://github.com/Vic-Godwin/VictorCompress/README.md). It allows you to read, search, and extract patterns like emails, phone numbers, dates, and file statistics from `.txt` files — including those decompressed by VictorCompress.

---


## ✨ Features

- 📂 Load `.txt` files instantly
- 🔍 Search for specific keywords or line starters
- 📊 Extract useful metadata:
  - File word count, character count
  - Word frequency tracking
  - Phone numbers, emails, and dates
- 🔄 Built-in **compress** and **decompress** engine for on-the-fly conversion using `zlib + base64`
- 🧠 Intelligent UI with dropdown options and dynamic outputs

---

## 🖼️ Interface Overview

- Top field to paste or browse a file path
- Text area shows results (search, file contents, or extracted data)
- Multiple buttons: **Read**, **Search**, **Convert**, **Extract**
- Combobox to select extraction category or action (e.g., `EMAIL`, `DATE`, `COMPRESS`, etc.)

---

## 🚀 Getting Started

### 📦 Requirements

This module uses:

```txt
Python >= 3.7
Standard Libraries: tkinter, re, os, base64, zlib, sys, time
External: None (except ttk for styling) if you're proficient in it, but i didn't use it for the VicReader
```

---

## 🧪 Example Usage

### 🔹 Launching the Reader
You can run it from terminal:

```bash
python vic_file_reader.py
```

### 🔹 Convert a File (Compress/Decompress)
1. Choose an action from the dropdown ("COMPRESS" or "DECOMPRESS")
2. Click the **Convert** button
3. The file is saved automatically as `compress_outputfile.txt or decompress_output.txt`. Then click readfile to reload view

```python
# Example of manual compression using compress_module
from compress_module import compress as com
compressed = com("your_file.txt")
```

---

## 📋 Sample Output: File Details
If you choose `FILE DETAILS` and search for `life`, you may see:

```
NUMBER OF WORDS IN FILE =  534

THE WORD 'LIFE' APPEARED 4 TIMES

NUMBER OF CHARACTERS IN FILE =  2893
```

---

## 🔎 Extracting Data
### 📧 Emails
```
Email 1: example@domain.com
Email 2: info@vicreader.io
```

### 📞 Phone Numbers
```
Phone Number 1: +234-809-123-4567
Phone Number 2: 08123456789
```

### 📆 Dates
```
Date 1: 25/06/2025
Date 2: 2024-10-13
```

---

## 📁 Project Tree Update

```
├── vic_file_reader.py         # ←SECOND VERSION This file (VicReader)
├── compress_module.py         # Compression engine
├── victor_logo_64x64.ico
├── victor_logo_64x64.png
├── LICENSE
├── README.md
├── requirements.txt
└── .gitignore
```

---

## 📘 License
This project is under the [MIT License](LICENSE).

---

## 🙌 About the Author
**Victor Godwin**  
🎯 Developer | 📚 Educator | ⚡ Innovator  
GitHub: [Vic-Godwin](https://github.com/Vic-Godwin)

---

## 🌟 Love this tool?
Star ⭐ the repo and [explore the full VictorCompress project here →](https://github.com/Vic-Godwin/VictorCompress)
