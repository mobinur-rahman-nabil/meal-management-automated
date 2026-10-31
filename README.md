# 🏨 Smart Hostel Analytics & Automated ETL Pipeline

An automated Business Intelligence and data pipeline built using **n8n**, **JavaScript**, and **Google Gemini** to ingest, process, and extract executive insights from 20 months of multi-sheet hostel operational records.

---

## 📊 The n8n Automation Architecture

Rather than reading through thousands of lines of raw JSON, here is the complete visual production pipeline driving this automation framework:

![n8n Workflow Automation Canvas](n8n-workflow-canvas.png)

### ⚙️ Workflow Breakdown
1. **Trigger:** Sequential disk ingestion reading multi-year Excel spreadsheets.
2. **Data Extraction:** Ingests raw `.xlsx` binaries and splits rows dynamically.
3. **Data Pre-processing (JS):** Cleans irregular formatting, maps empty variables, and aggregates active-day logs.
4. **AI Processing Layer:** Feeds structured JSON data into the **Google Gemini Chat Model** using optimized prompt templates for qualitative auditing.
5. **Report Formulation (JS):** Synthesizes structural mathematical outputs and AI insights into a responsive HTML/CSS executive dashboard layout.

---

## 🚀 The Core Problem & Solution

* **The Problem:** Manually auditing 20 individual monthly Excel sheets containing **844+ rows** of compound variables (individual consumption, costs, dynamic active-days) for members (*Nabil, Imran, Sanim, Raiyan*) is inefficient and open to human calculation error.
* **The Solution:** This pipeline replaces human calculations entirely. It transforms raw file structures into structural metrics, passing complex contextual logs to an LLM to evaluate trends in food wastage, active days, and optimized expense distribution instantly.

---

## 🛠 Tech Stack & Concepts Demonstrated

* **Orchestration & Automation:** n8n (Advanced workflow scheduling, local file nodes, and node execution chains).
* **Scripting & Engineering:** JavaScript (Binary data mapping, JSON transformation arrays, and dynamic object formatting).
* **Generative AI Engineering:** Google Gemini API (Structured prompting, JSON formatting schemas, and token context optimization).
* **Database & File Handling:** Excel Data Processing, Multi-sheet extraction, and Dynamic IO.
* **Frontend Reporting:** HTML5 & CSS3 (Automated generation of clean reporting metrics).

---

## 📂 Repository Layout

```text
├── HostelMeal_n8n_workflow.json  # Complete exportable production automation file
├── Hostel_Report.html            # Example generated dynamic analytical dashboard
├── n8n-workflow-canvas.png       # Visual architecture design screenshot
└── README.md                     # Project blueprint & comprehensive technical overview
```

---

## ⚡ Quick Deployment Guide

### Prerequisites
* A running **n8n** instance (Local Desktop app or Cloud instance).
* A valid **Google Gemini API Key**.

### Setup Instructions
1. Clone this repository or copy the `HostelMeal_n8n_workflow.json` data.
2. In your n8n workspace, click **Import from File** and upload the `.json` file.
3. Update the *Read/Write Files from Disk* node path to target your target directory containing your excel spreadsheets.
4. Insert your Gemini API Key credentials into the *Google Gemini Chat Model* connection card.
5. Execute the pipeline. The system will dynamically generate and save an analytical `Hostel_Report.html` dashboard directly to your local file path.
