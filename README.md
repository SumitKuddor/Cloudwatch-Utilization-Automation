# AWS CloudWatch Utilization Automation (Local Machine)

This project automates AWS CloudWatch utilization reporting using Python and runs entirely on a local machine.
It eliminates manual reporting and avoids additional AWS service costs.

---

## 🚀 Features
- Collects EC2 and RDS utilization metrics from AWS CloudWatch
- Generates Excel and Word reports with graphs
- Runs on a local machine using AWS CLI & IAM (read-only access)
- Can be scheduled using Cron (Linux) or Task Scheduler (Windows)
- Cost-effective alternative to Lambda-based automation

---

## 🛠 Tech Stack
- Python 3.x
- AWS CLI
- AWS CloudWatch
- IAM (Least Privilege)
- Excel & Word report generation

---

## 📁 Project Structure

aws-cloudwatch-utilization-reporter/
├── report_generator.py
├── inventory.json
├── requirements.txt
├── images/
│ ├── cpu.png
│ ├── memory.png
│ └── disk.png
└── reports/
├── excel/
└── word/

## 🔐 Prerequisites
- Python 3.9+
boto3
python-docx
openpyxl
matplotlib
pandas
- AWS CLI configured
- IAM user with read-only access to:
  - EC2
  - RDS
  - CloudWatch

## ▶️ How to Run
python report_generator.py
