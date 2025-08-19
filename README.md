# Automated Customer Feedback System (Forms + Power Automate + Excel + Power BI)

A production-style workflow that collects customer feedback via **Microsoft Forms**, analyzes **sentiment with AI** in **Power Automate**, logs records to **Excel**, and visualizes insights in **Power BI** with a dynamic dashboard and an **Insights** button.

> **Try it:** Submit feedback here → **https://lnkd.in/g2xxKBZP**  
> **See the deck:** **https://www.canva.com/design/DAGpFyjLn4U/VnK-0q59HLUONJCI_IA1sQ/view?utm_content=DAGpFyjLn4U&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=h0aeb1460ee**

---

##  Overview
This project automates the end-to-end feedback cycle:
1. **Collect** feedback using Microsoft Forms.
2. **Analyze** sentiment (Positive / Neutral / Negative) with AI in Power Automate.
3. **Act** on results: auto-email support for Negative feedback; append all submissions to Excel.
4. **Visualize** trends, volumes, and categories in Power BI with near real-time refresh.

**Why it matters:** Faster response to negative feedback, consistent data capture, and a single source of truth for customer sentiment.

---

##  Architecture
- **Input:** Microsoft Forms → customer name, email, feedback text, (optional) rating/category.  
- **Automation:** Power Automate flow triggers on new submission, gets response details, runs AI sentiment, branches by condition, writes to Excel, emails support when needed.  
- **Storage:** Excel (OneDrive/SharePoint) table as system of record.  
- **Analytics:** Power BI connected to the Excel table; interactive dashboard with Trends, Sentiment Breakdown, and Insights button.

##  Test Scenarios
- **Positive feedback** → Row added, no email sent  
- **Neutral feedback** → Row added, no email sent  
- **Negative feedback** → Row added **and** email alert sent  
- **Date variations** → Normalized into a consistent format  

---

##  Power BI Dashboard
**Key visuals include:**  
- **Sentiment Over Time** (line/area chart)  
- **Sentiment Breakdown** (donut/bar chart)  
- **Feedback Volume by Day/Week**  
- **Negative Feedback Details** (table)  
- **Insights Button** with Smart Narrative for automated summaries
- **Link** -https://app.powerbi.com/view?r=eyJrIjoiYjY5MjQxMDMtYmFjMC00ZDkzLTkzYjYtNzg2NzBkN2YyMGY2IiwidCI6ImE2ZGJkZGRlLTU3OTgtNGViYS1hNWE4LTc4ODA3ZTgyZDllYiJ9

