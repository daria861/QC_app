# QC Website Audit & Feedback Generator

A lightweight, single-file interactive web application designed for Quality Assurance (QA), Designers, and Developers to quickly audit websites, collect feedback, attach screenshots, and export visual report documents (.docx, .html, and PDF).

---

## Features

- **Inline Editing**: Click or double-click any cell (Page Name, Page URL, Element, Description) to edit directly in the browser.
- **Direct Clipboard Screenshot Uploads**: Select an image cell and paste screenshots directly from your clipboard using `Ctrl+V` (or `Cmd+V`), drag and drop image files, or upload through the file picker.
- **Status & Action Tag Management**:
  - **Status Pills**: `To Do`, `In Review`, `Done`, `Waiting for`.
  - **Action To Options**: Preset tags (`Frontend`, `Backend`, `QC`) with the ability to add custom team members or departments on the fly.
- **Image Scale & Lightbox Modal**: Click any screenshot thumbnail to expand and view full-resolution image details.
- **Multi-Format Export Options**:
  - **Export Word (`.docx`)**: Generates a landscape Microsoft Word document formatted cleanly for sharing with developers or clients.
  - **Export Interactive HTML**: Exports a single-file standalone web page where Status dropdowns and Description fields remain active and images remain click-to-zoomable.
  - **Print / Save as PDF**: Formatted print layout (`@page { size: landscape; }`) that reflows table columns cleanly without truncation.
- **Local Persistence & Zero Setup**: Automatically saves all active report data to your browser's `localStorage` so your work isn't lost on page refresh.

---

## Requirements

No backend server, Node.js installation, or build process required!

The app uses standard web browser technologies along with CDN libraries:
- **Tailwind CSS** (for styling)
- **html-docx-js** & **FileSaver.js** (for Word file generation)
- **FontAwesome** (for interface icons)

---

## Quick Start Guide

### 1. Running the App
1. Download or copy `index.html` to your computer.
2. Double-click `index.html` to open it in any modern web browser (Google Chrome, Firefox, Safari, Microsoft Edge, Brave).

> **Note for Google Drive users:** If you upload `index.html` to Google Drive, download the file to your computer first before opening it, or use a Google Drive HTML Viewer app extension.

### 2. Using the Dashboard
1. **Edit Title**: Click on the orange header bar text (*"Feedback to dev"*) to customize the report title.
2. **Add Issues**: Click **`+ Add Row`** to insert a new feedback item.
3. **Attach Screenshots**: Click inside the **Description Image** cell and press `Ctrl+V` / `Cmd+V` to paste a screenshot directly from your clipboard, or click **Upload**.
4. **Assign Items**: Set the **Status** pill color and select who needs to address the item (**Action To**).
5. **Export Report**: Click **`Export Word (.docx)`** or **`Export HTML`** in the top toolbar to share the generated document with your development team.

---

## File Structure

```text
├── index.html        # Main web application logic, styles, and templates
└── README.md         # Documentation
