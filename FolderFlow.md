# 🗂️ FolderFlow: Modern Folder Management Suite

FolderFlow is a comprehensive toolkit for converting, modifying, and reconstructing folder structures through text-based representations. This all-in-one solution enables seamless folder manipulation with a clean, modern interface.

---

## 🛠️ Core Tools

### 📂 Folder to TXT Converter
- Convert folder hierarchies into structured text documents  
- Preserve file content and indentation  
- Local browser processing for privacy

### 🔍 TXT Replacer
- Find/replace text across entire folder structures  
- Real-time preview and match counting  
- Case-sensitive search options

### 📄 TXT to Files Converter
- Reconstruct folders from text-based representations  
- Preview file hierarchy before generation  
- Export as individual files or ZIP archives

---

## ⚙️ Supporting Infrastructure

- **Flask Backend (`FolderFlow Home.py`)**
  - Local server with ZIP monitoring  
  - Automatic browser launch  
  - Folder extraction system  

- **Tkinter Folder Picker (`pick_location.py`)**
  - Native OS folder selection dialog

- **Success Notification (`exit.vbs`)**
  - Windows popup after successful extraction

- **Modern UI**
  - Dark mode aesthetic  
  - Responsive layout  

---

## ✨ Technical Highlights

- **Client-Side Processing:** All conversions happen locally in the browser  
- **Seamless Workflow:** Push processed data between tools via `localStorage`  
- **Visual Feedback:** Progress bars, file counters  
- **Responsive Design:** Mobile-friendly interface  
- **ZIP Automation:** Monitors system folders for new ZIPs

---

## 🧭 Getting Started

1. Run `FolderFlow Home.py` to launch the local server  
2. Open `http://127.0.0.1:5000/` in your browser  
3. Use the nav menu to access:
   - 📂 Folder to TXT
   - 🔁 TXT Replacer
   - 📄 TXT to Files

---

FolderFlow simplifies complex folder operations while keeping everything **local & private** — ideal for developers, content managers, and anyone working with structured file systems.

---

## 🤖 Bonus

Yes, parts of this were co-developed with AI — because two braincells are better than one.

---

## 📜 License

This document is licensed under  
**[CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/)**  
> You can read it. You can cry over how good it is. But you can’t resell or remix it.

