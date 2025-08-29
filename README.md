Executive Gantt Chart Generator

A single-file, zero-dependency, interactive web application for generating clean and professional-looking Gantt charts. This tool is designed to quickly turn project data from a spreadsheet into a high-quality visual perfect for executive summaries, portfolio reviews, and presentations.
Key Features

    Single HTML File: No servers, no dependencies, no build steps. Just one html file you can open anywhere.

    Paste and Go: Simply copy data from Excel or Google Sheets and paste it directly into the application.

    Automatic 5-Phase Generation: If you only provide a project's start and end date, the tool will automatically generate a standard 5-phase waterfall (Prepare, Design, Build & Test, Deploy, Stabilize).

    Fully Interactive: Dynamically adjust the timeline's zoom, row height, and other visual parameters to get the perfect view.

    Responsive Layout: The chart automatically fits your browser window and redraws on resize.

    High-Quality Export:

        SVG Export: Get a crisp, scalable vector graphic for further editing.

        High-Resolution PNG Export: Download a high-quality, presentation-ready PNG with a single click.

    Clear Visual Grouping: Projects are automatically grouped by stream, with vertical labels and alternating background shades for readability.

How to Use

    Download: Download the gantt.html file from this repository.

    Open: Open the gantt.html file in your web browser (e.g., Chrome, Firefox, Edge). You can do this by double-clicking the file or dragging it into a browser window.

    Paste Your Data: Paste your project data from a spreadsheet into the large text area at the bottom.

    Render & Customize: The chart will render automatically. Use the controls in the header to adjust the view to your liking.

    Download Your Chart: Click "Download SVG" or "Download PNG" to get your high-quality export.

Input Data Format

The application accepts tab-separated (TSV) or comma-separated (CSV) data. You can paste it directly from any spreadsheet software. The header row is optional and will be ignored.

There are two primary formats you can use:
1. With Automatic 5-Phase Generation

If you only provide a project's overall start and end dates, the tool will automatically create the 5 standard phases for you.

Columns: Stream, Project, Start, End
code Code
IGNORE_WHEN_COPYING_START
IGNORE_WHEN_COPYING_END

    
Cross-stream  Project Phoenix   2025-01-15  2025-09-01
P2P           Vendor Portal     2025-02-01  2025-09-30
A2G           HR Platform       2025-04-10  2025-12-31

  

2. With Specific Phases

If you want to define each phase manually, use this format.

Columns: Stream, Project, Phase, Start, End, (Optional) Color
code Code
IGNORE_WHEN_COPYING_START
IGNORE_WHEN_COPYING_END

    
Cross-stream,Project Phoenix,Prepare,2025-01-15,2025-02-15
Cross-stream,Project Phoenix,Design,2025-02-10,2025-04-10,#34d399
P2P,Vendor Portal,Build & Test,2025-04-15,2025-08-15

  

Author

Created by Jakub Grzywa
License

This project is licensed under the MIT License.
