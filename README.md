# Smart Hostel Management & Analytics Pipeline

An automated Business Intelligence and data pipeline built using **n8n**, **JavaScript**, and **Google Gemini** to ingest, process, and analyze 20 months of hostel operational data.

## 🚀 Project Overview
Managing multi-sheet Excel records for a hostel spanning nearly two years (844+ rows across 20 monthly sheets) is tedious and prone to manual error. This project automates the entire auditing process—from raw spreadsheet ingestion to AI-powered analytical reporting—eliminating manual math and delivering executive-ready insights instantly.

## 🛠️ Key Features
- **Automated ETL Pipeline:** Built an end-to-end n8n workflow to ingest and aggregate complex multi-sheet Excel workbooks.
- **Data Transformation & Scripting:** Utilized custom JavaScript nodes to handle data normalization, cleaning, and JSON/binary payload structuring.
- **Generative AI Integration:** Programmatically integrated Google Gemini within the automation workflow to perform advanced qualitative analysis and pattern recognition.
- **Member Performance Tracking:** Automatically aggregates individual statistics and consumption metrics for hostel residents (Nabil, Imran, Sanim, Raiyan).
- **Executive Dashboard Reporting:** Synthesizes raw calculations into a structured, clean HTML/CSS analytical report focused on food waste reduction and active-day tracking.

## 📂 Repository Structure
- `hostel_analytics_workflow.json` - The complete, exportable n8n workflow automation file.
- `Hostel_Dashboard.html` - The generated visual management report template.

## ⚙️ How to Use
1. Import `hostel_analytics_workflow.json` into your local or cloud-hosted **n8n** instance.
2. Link your source Excel file containing the monthly meal records.
3. Configure your API key for Google Gemini within the AI nodes.
4. Execute the workflow to automatically generate and extract the latest analytical HTML report.