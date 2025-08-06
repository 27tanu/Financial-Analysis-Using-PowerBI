Project Title: Financial Project Automation
🧾 Overview
This project automates the end-to-end process of managing emails related to credit score data, extracting attachments, processing the data, and visualizing insights via Power BI. It integrates Microsoft Outlook rules, Power Automate, Google Drive API, Python scripting, and Power BI to create a seamless and efficient financial reporting pipeline.

📚 Table of Contents
Introduction

Technologies Used

Workflow Description

Data Transformation

Power BI Dashboard

Client Requirements

Installation and Setup

Usage

Contributing

License

🔍 Introduction
Financial Project Automation was developed to streamline and optimize the daily workflow of processing multiple financial data files received via email. It automates:

Email filtering,

Attachment handling,

File storage and retrieval,

Data transformation,

Visual dashboard generation.

This project has significantly reduced manual labor, minimized errors, and improved the timeliness and accuracy of financial insights.

🛠 Technologies Used
Microsoft Outlook – Email filtering via rules

Power Automate – Attachment extraction and cloud upload

Google Drive API – File access and retrieval

Python – Data fetching, cleaning, transformation

Power BI – Data visualization and dashboarding

🔄 Workflow Description
📧 Email Rule Creation

A rule in Outlook moves any email containing "Credit Score" in the subject or body to a Financial Project Folder.

📂 Attachment Extraction

Power Automate detects emails in the folder, extracts the attachments, and uploads them to a designated Google Drive folder.

🔗 Google Drive API Integration

A Python script uses the Google Drive API to fetch newly uploaded files into the local system for processing.

🧹 Data Processing (ETL)

Files are merged, cleaned, and transformed using Python:

Data types corrected

Nulls handled

Business logic applied to enrich the dataset

📈 Dashboard Creation in Power BI

The cleaned data is fed into Power BI, where an interactive dashboard is built to reflect real-time insights as per the client’s detailed requirements.

🧼 Data Transformation
✅ Data Type Conversion: Ensuring numerical, categorical, and date fields are correctly typed.

✅ Null Value Handling: Imputed missing values using relevant business logic.

✅ Value Replacement & Enrichment:

Mapped coded values to readable labels

Created new features (e.g., age group, credit score category)

Applied transformations for LTV calculations and grouping logic

📊 Power BI Dashboard
The dashboard includes:

Key metrics (e.g., Avg. Annual Income, Credit Utilization)

Age group segmentation and credit score distributions

Loan type dispersion visuals

Customer potential and LTV-based promotion mapping

The dashboard has improved decision-making efficiency and reduced client operational costs.

🧾 Client Requirements
The client required insights on:

Demographics, payment behavior, and product preferences

LTV score computation and promotion rules

Credit mix and behavioral trends

Potential customer segmentation

Loan type popularity analysis

📄 Refer to Financial Dashboard.docx for full requirement documentation.

⚙️ Installation and Setup
Clone the Repository

bash
Copy
Edit
git clone https://github.com/yourusername/financial-project-automation.git
Set Up Dependencies

Python 3.x

Install required Python libraries:

bash
Copy
Edit
pip install pandas numpy google-api-python-client oauth2client
Configure Services

Set up Outlook rule for email filtering

Set up Power Automate to save attachments to Google Drive

Generate credentials for Google Drive API

Power BI

Open the .pbix file (transforming.pbix) in Power BI Desktop

Refresh data sources to view latest insights

▶️ Usage
Run the Python script to fetch and clean the files:

bash
Copy
Edit
python fetch_and_transform.py
Open Power BI and refresh the data model.

Interact with the dashboard visuals to explore insights.

Update or append new data using the same pipeline.

🤝 Contributing
Have ideas to improve the project? Contributions are welcome!

Fork the repository

Create a new feature branch

Submit a pull request for review

📄 License
This project is licensed under the MIT License.
See the LICENSE file for more details.

