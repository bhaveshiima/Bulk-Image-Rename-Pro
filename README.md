# Bulk Image Rename Pro

> **An Initiative by Vikram Sarabhai Library, IIM Ahmedabad**

A lightweight, browser-based tool for renaming large collections of images in bulk using an Excel workflow — no installation, no server, no data upload required. Everything runs entirely in your browser.

---

## Features

- **Drag-and-drop upload** — select multiple images at once; thumbnails appear instantly
- **Visual preview grid** — see all images with editable filename inputs
- **Excel workflow** — export filenames to a spreadsheet, fill in new names, re-import in one click
- **Smart matching** — import matches images by original filename, so row order in Excel doesn't matter
- **Individual rename** — edit any single filename directly in the preview card
- **Individual delete** — remove a single image from the queue without clearing all
- **Live duplicate detection** — conflicting names turn red instantly; download is blocked until resolved
- **Locked extension** — original file format (`.jpg`, `.png`, etc.) is always preserved
- **Download ZIP** — all renamed images packaged into a single `Renamed_Images.zip`
- **Dark / Light theme** — toggle persisted across browser sessions
- **Fully offline** — works without internet after the page loads

---

## How to Use

### Option A — Run Locally (Recommended)

1. **Download** the repository as a ZIP or clone it:
   ```
   git clone https://github.com/YOUR_USERNAME/bulkimagerename.git
   ```
2. Open the `index.html` file directly in any modern browser (Chrome, Edge, Firefox).
3. No server needed — just double-click the file.

### Option B — Run via Local Server (XAMPP / VS Code Live Server)

1. Place the `index.html` file inside your server's web root (e.g. `C:\xampp\htdocs\bulkimagerename\`).
2. Start Apache and visit `http://localhost/bulkimagerename/`.

---

## Step by Step Workflow

### Step 1 — Upload Your Images

Drag and drop image files onto the **upload zone** in the left sidebar, or click the zone to open your file picker. Select as many files as you need — they will appear as thumbnail cards sorted alphabetically.

> Supports JPG, PNG, WEBP, GIF and all common image formats.

---

### Step 2 — Export List

Click the **Export List** button. An Excel file (`ImageList.xlsx`) will be downloaded with two columns:

| Column | Description |
|--------|-------------|
| `Original_Filename` | Your original image filenames — **do not edit this column** |
| `New_Filename` | Leave blank — **fill in your desired new names here** |

Open the file in Excel or Google Sheets, fill in the `New_Filename` column for each image, and save the file.

---

### Step 3 — Import List

Click the **Import List** button and select the saved Excel file. The tool will instantly read the new names and apply them to the matching images on screen.

> Names are matched by `Original_Filename`, so even if you reorder rows in Excel, the correct name always goes to the correct image.

---

### Step 4 — Download ZIP

Click the **Download ZIP** button in the toolbar. All your renamed images will be packaged into `Renamed_Images.zip` and saved to your device. Extract the ZIP — all photos will have their new names with their original formats preserved.

---

## Screenshots

> *(Add screenshots of the tool here)*

---

## File Structure

```
bulkimagerename/
├── index.html      ← The entire application (HTML + CSS + JS in one file)
├── README.md
├── project.md      ← Project overview and architecture
└── skill.md        ← Technical skills and implementation notes
```

---

## Browser Compatibility

| Browser | Status |
|---------|--------|
| Chrome 90+ | ✅ Fully supported |
| Edge 90+ | ✅ Fully supported |
| Firefox 88+ | ✅ Fully supported |
| Safari 14+ | ✅ Supported |

---

## Technology Stack

| Technology | Purpose |
|------------|---------|
| HTML5 / CSS3 / Vanilla JS | Core application — no frameworks |
| [SheetJS (xlsx)](https://sheetjs.com/) | Excel file read/write in the browser |
| [JSZip](https://stuk.github.io/jszip/) | ZIP file creation and download |
| [Font Awesome](https://fontawesome.com/) | UI icons |
| [Google Fonts](https://fonts.google.com/) | Inter & JetBrains Mono typefaces |

---

## Privacy

All processing happens **locally in your browser**. No images, filenames, or any data are ever sent to a server. Closing the tab clears everything.

---

## Credits

**Designed and developed by** Sunit, Library Trainee (Batch : 2025-26)
**Mentored by** Bhavesh Patel, Sr Library Professional – IT Applications
**Vikram Sarabhai Library, IIM Ahmedabad**

---

## License

This project is open for use within academic and library contexts. Feel free to adapt it for your institution's needs.
