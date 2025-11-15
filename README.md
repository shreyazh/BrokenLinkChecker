# 🔗 Broken Link Checker – GUI + JS Rendering + Multithreading + exe Builder

A powerful, modern Broken Link Checker desktop application built with **Python**, featuring:

- Full **GUI** (Tkinter)
- **JS-rendering support** (Playwright) — Works with React, Next.js, Vue, Angular, etc.
- **Multithreading** for extremely fast link scanning
- **Broken links highlighted in red**
- **Filter** to show only broken links
- **Column sorting**
- **Export broken links to CSV**
- **Copy broken links to clipboard**
- **Optional green progress bar**
- Works as a **standalone Windows .EXE** (PyInstaller)

---

# 🚀 Features

## 1. JavaScript Rendering (Next.js / React)
Uses **Playwright Chromium** to render dynamic pages and extract real DOM links.

## 2. Multithreaded Link Checker
Link checks run in parallel using `ThreadPoolExecutor`, drastically reducing scan time.

## 3. GUI Application
Built with Tkinter:
- URL input
- Check links button
- JS rendering toggle
- Status bar
- Progress bar
- Link results table

## 4. Broken Link Identification
Broken links are:
- Highlighted **red**
- Filterable via “Show Broken Only”
- Exportable and copyable

## 5. CSV Export & Clipboard Copy
Useful for audits, reports, SEO analysis, QA testing.

## 6. Sorting
Click table headers to sort by:
- URL
- Status
- Broken?

## 7. EXE Support
Can be compiled to a **standalone Windows application** via PyInstaller.

---

# 📦 Installation

### 1. Install dependencies

```bash
pip install playwright requests beautifulsoup4
python -m playwright install chromium
pip install pyinstaller
```

### 2. Running
```bash
python linkCheckGUI.py
```

### 3. Building a Standalone .exe 
```bash
python -m PyInstaller --onefile --noconsole linkCheckGUI.py
```
