# 🧩 Process Flow Visualizer

Interactive web-based process flow visualizer with swim lane diagrams. Upload Excel data or enter manually, export to PDF/Excel. Built with D3.js and vanilla JavaScript.

🖼️ Screenshot
![Process Visualizer Screenshot](screenshot.png)

A lightweight, interactive, browser-based tool for visualizing process workflows using swimlanes and process steps. This visualizer supports manual data entry or Excel import, and allows exporting the diagram as both Excel and PDF.

## 🚀 Features

- 🖼️ **Swimlane-style process visualization** using D3.js
- 📥 **Excel upload support** (XLSX and XLS)
- ⌨️ **Manual data entry** through a dynamic table
- 📤 **Export options**: Download process data as Excel or diagram as PDF
- 🎨 **Dynamic rendering** with smart text wrapping and connectors
- 🛠️ **Editable workflow name** and real-time updates

## 📁 File Structure

This project consists of a single HTML file:

```
process-visualizer-v4.html
```

## 🛠️ Tech Stack

- [D3.js v7](https://d3js.org/)
- [SheetJS (xlsx)](https://github.com/SheetJS/sheetjs)
- [html2canvas](https://html2canvas.hertzen.com/)
- [jsPDF](https://github.com/parallax/jsPDF)

## 🧪 Usage

### Option 1: Manual Data Entry

1. Open the `process-visualizer-v4.html` file in any modern browser.
2. Enter steps in the table: Order, Swim Lane, Step Name, and Description.
3. Click **Generate Diagram**.

### Option 2: Excel Upload

1. Prepare your Excel file with the following format:
    - Row 1 (optional): `Workflow Name:` followed by your title.
    - Skip 2 rows.
    - Header: `Order`, `Swim Lane`, `Step Name`, `Description`
    - Subsequent rows: your process steps.
2. Upload via the **Upload Excel File** button.
3. Diagram generates automatically.

### Exporting

- Click **Download as Excel** to save the workflow data.
- Click **Download as PDF** to export the diagram.

## 📄 Sample Excel Format

```text
Workflow Name:	Customer Onboarding
Created:	2025-06-04

Order	Swim Lane	Step Name	Description
1	Sales	Lead Generation	Generate new leads
2	Marketing	Qualification	Qualify leads
```

## 📌 Customization

- To update style or layout, modify the embedded CSS and `ProcessVisualizer` class in the `<script>` tag.
- Layout and spacing constants (like shape size, padding) are defined in the `this.config` object.

## 🧑‍💻 Author

**Asim**

> Creative solutions for visualizing complex workflows made simple.

## 📄 License

MIT License. Free for personal and commercial use.
