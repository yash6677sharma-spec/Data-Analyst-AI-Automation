# Data Analyst AI Automation

An automated data-analysis workflow built with **n8n**.

## What it does

- Accepts CSV or Excel (.xlsx) uploads through an n8n form.
- Detects the uploaded file type and extracts the data.
- Cleans the dataset by trimming text, normalizing empty values, removing empty rows, and removing exact duplicates.
- Generates a cleaned Excel report.
- Computes automatic business insights such as totals, averages, minimums, maximums, counts, distinct values, and top categorical values.
- Generates a separate Excel insights report.
- Emails both Excel files through Gmail.

## Workflow

```text
Upload Data File
      ↓
Prepare File
      ↓
Route By File Type
   ↙         ↘
 CSV        Excel
   ↘         ↙
      Clean Data
          ↓
 Generate Excel Report
          ↓
   Compute Insights
          ↓
Generate Insights Excel
          ↓
 Assemble Attachments
          ↓
     Email Report
```

## Live n8n Form

https://yash9999.app.n8n.cloud/form/b8b1cde6-6b41-4e58-80e0-5b314e0878f3

## Repository

- `n8n/Upload File to Excel Report.json` — exported n8n workflow
- `README.md` — project documentation

## Technologies

- n8n
- JavaScript
- CSV / Excel
- Gmail

## Author

Yash Sharma
