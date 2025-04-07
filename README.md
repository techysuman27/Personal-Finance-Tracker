# 💸 Personal Finance Tracker Dashboard (Excel)

An interactive and visually appealing **Personal Finance Dashboard** built in **Microsoft Excel** to monitor income, expenses, and spending habits. The project is aimed at promoting smarter personal finance management through effective data visualization and automated KPI tracking.

---

## 📸 Visual Preview

![Finance Dashboard Preview](./asset/PersonalFinanceDashboard.png)

---

## 📂 Project Structure & Workflow

This Excel-based project follows a **3-layer architecture**:

1. **📑 Dataset Layer** (`Data` sheet): Contains raw monthly records of income and expenses
2. **📊 Pivot Analysis Layer** (`Calculations` sheet): Builds dynamic Pivot Tables for summarization
3. **📈 Dashboard Layer** (`Dashboard` sheet): Visualizes insights using charts, cards, and graphs

---

## 🧾 Dataset Description

The dataset used in this project captures real-life finance entries across various categories:

| Column Name      | Description                                   |
|------------------|-----------------------------------------------|
| `Date`           | Date of the transaction (dd-mm-yyyy)          |
| `Type`           | Income or Expense                             |
| `Category`       | Spending/earning category (e.g. Housing, Job) |
| `Amount`         | Transaction amount                            |
| `Source`         | Platform/source of income (YouTube, Job, etc) |
| `Day`            | Weekday name (Mon, Tue, etc.) for trend analysis |
| `Month`          | Month name (Jan, Feb, etc.) for trend charts  |

---

## 🧪 Feature Engineering (Excel Formula-Based)

To enhance analysis and build insightful visualizations, we performed **feature extraction** from the raw `Date` column:

| New Column | Formula Used (in Excel) | Description |
|------------|--------------------------|-------------|
| `Month`    | `=TEXT(A2, "mmm")`       | Extracts 3-letter month name from Date |
| `Day`      | `=TEXT(A2, "ddd")`       | Extracts weekday name (Mon, Tue, etc.) from Date |

These columns are crucial for:
- **Monthly trend analysis** in bar charts
- **Weekday spending pattern** visualization
- **Grouping data** in Pivot Tables dynamically

> 🧠 These transformations allow the dashboard to stay dynamic, filterable, and timeline-aware.

---

## 🔍 Primary Analysis (Pivot Table Layer)

The `Calculations` sheet is dedicated to:
- Creating **Pivot Tables** for income and expense aggregation
- Calculating KPIs like **total income**, **total spending**, **available balance**
- Deriving **monthly** and **weekly trends**
- Feeding structured results into the dashboard using linked cells

💡 This sheet acts as the engine powering the dashboard – update the `Data` sheet, and everything auto-updates.

---

## 📊 Key Dashboard Metrics

| Metric                  | Value     |
|------------------------|-----------|
| 💰 Available Balance   | $35,249   |
| 📥 Total Income        | $65,440   |
| 📤 Total Spending      | $30,191   |
| 🧾 Max Income Source   | Data with Decisions - $50,000 |
| 🏠 Top Spending        | Housing - $9,000 |
| 📅 Max Weekly Spending | Monday - Highest |
| 📆 Max Monthly Income  | October - $5,000 |

---

## 🧩 Dashboard Features

- 💳 **Credit Card-Style Balance Card** showing available funds
- 📈 **Monthly Trends** (bar chart) for income and expenses
- 📊 **Top 5 Expense Categories** visualized as colored KPI blocks
- 🕒 **Weekly Trend Chart** to analyze weekday spending habits
- 🍩 **Income Source Distribution** with percentage-wise donut chart
- 🌘 **Dark Theme Dashboard** for a clean and modern user experience


## 🛠 Tools & Techniques Used

| Tool              | Purpose                                 |
|------------------|------------------------------------------|
| Microsoft Excel  | Dashboard building, charts, formulas     |
| Pivot Tables      | Data aggregation, filtering              |
| Excel Charts     | Column, Donut, Line, KPI layout          |
| Conditional Formatting | Highlighting spending levels       |
| Excel Formulas   | SUMIFS, MAX, TEXT, VLOOKUP, dynamic ranges     |
| Icons/Emojis     | Visual enhancement of sections/cards     |

---

## 🚀 How to Use This Dashboard

1. **Download or Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/personal-finance-tracker.git
