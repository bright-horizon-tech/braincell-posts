
# ✏️ Font Previewer: Instant .TTF Typing & Testing

Font Previewer is a lightweight desktop utility for instantly loading and testing TrueType fonts (`.ttf`) without installing them system-wide. Whether you're a designer, typographer, or just font-curious, this tool lets you type, adjust, and save your creations on the fly.

---

## 🛠️ Core Tools

### 📥 Font Loader
- Load any local `.ttf` file directly from disk  
- Instantly apply it in the editor without permanent installation  
- Supports multiple TrueType families

### ⌨️ Live Font Editor
- Type and preview text with the selected font immediately  
- Adjustable font size (8–120pt) via a smooth slider  
- Real-time rendering in the preview area

### 🖼️ Image Exporter
- Save typed text as a `.png` image  
- Preserves the loaded font style and size  
- White background for clean, shareable output

---

## ⚙️ Supporting Infrastructure

- **PyQt5 GUI (`FONT PREVIEWER.py`)**  
  - Modern, responsive interface  
  - Cross-platform window layout  
  - Native file dialogs for loading fonts and saving images

- **Live Font Application**  
  - Uses `QFontDatabase` to register fonts temporarily  
  - Ensures system fonts remain untouched

- **Error Handling**  
  - Alerts for invalid or missing files  
  - Prevents crashes during save/export

---

## ✨ Technical Highlights

- **No Installation Required:** Fonts are loaded temporarily into the app session  
- **Cross-Platform:** Works on Windows, macOS, and Linux (PyQt5)  
- **Clean UI:** Minimal controls, maximum space for creative typing  
- **Dynamic Font Sizing:** Slider-based adjustments without losing context  
- **Local Processing:** No internet needed, all rendering happens locally

---

## 🧭 Getting Started

1. **Install dependencies**:  
  ``` pip install PyQt5 ```

3. **Run the program**:

```   python FONT\ PREVIEWER.py ```

4. **Load a font**:

   * Click **Load .ttf** and select a TrueType font file

5. **Type and adjust**:

   * Type in the editor and adjust size with the slider

6. **Save as image**:

   * Export your design as a `.png` image

---

Font Previewer makes it ridiculously easy to experiment with typefaces in real time — perfect for quick mockups, design tests, or font reviews.

---

## 🤖 Bonus

Yes, parts of this were crafted with AI — because even fonts deserve a little machine learning love.

---

## 📜 License

This document is licensed under
**[CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/)**

> You can preview it, you can type in it, but you can’t resell or remix it without asking.
