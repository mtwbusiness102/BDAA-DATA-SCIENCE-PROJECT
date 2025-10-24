# 🧠 Global Data Breaches: Exploring Patterns, Impact, and Trends (2004–2024)

![Data Breach Banner](./images/data_breach_banner.png)

## 📘 Overview
This project analyzes **global data breach incidents** from **2004–2024**, identifying key patterns across sectors, breach methods, and years.  
Using Python for exploratory data analysis (EDA), the project highlights how cyber vulnerabilities have evolved and which industries face the greatest risk exposure.

> This project was created for a **Data Science / Cybersecurity portfolio** and designed to align with the **BDAA Project Poster Template**.

---

## 🎯 Problem Statement
Data breaches continue to compromise billions of personal records worldwide, causing financial loss, reputational harm, and legal consequences.  
This project aims to answer the following key questions:
- Which **industries** are most frequently targeted?
- What are the **most common breach methods**?
- How have **breach frequencies and sizes** changed over time?
- What **patterns or outliers** exist in global data exposure?

By uncovering these patterns, this project helps raise awareness of systemic risks and emphasizes the importance of proactive cybersecurity strategies.

---

## 🧩 Dataset

**Source:**  
Open-source *Balloon Race Data Breaches* dataset containing 417 verified incidents.  
Each record includes:
- Organization name  
- Year of breach  
- Sector / industry  
- Method of breach  
- Records lost  

**Total Records Lost:** ≈ **81 billion**  
**Time Range:** 2004–2024  

> Dataset cleaned and preprocessed in Python (Pandas), with missing values handled and breach counts aggregated by category.

---

## 🧠 Methodology

### 🧹 Data Cleaning
- Removed duplicate entries and inconsistent values.  
- Normalized breach method categories (e.g., “Hacked,” “Poor Security,” “Oops!”).  
- Converted “Records Lost” to numeric values for aggregation.  

### 📊 Exploratory Data Analysis (EDA)
- Visualized **breach counts per year**, **sector distribution**, and **breach methods**.  
- Identified outliers and trends using descriptive statistics.  
- Ranked top breaches by total records lost.

### 🛠️ Tools Used
- **Language:** Python  
- **Libraries:** pandas, numpy, matplotlib, seaborn  
- **Environment:** Jupyter Notebook  

---

## 📈 Key Findings (Results)

| Metric | Value |
|--------|--------|
| Total Breaches | 417 |
| Total Records Lost | ~81,000,000,000 |
| Most Common Method | Hacked |
| Peak Breach Year | 2019 |
| Top Sector | Web / Technology |

### 🔍 Insights
- **Hacking** remains the dominant breach vector (65%+ of all cases).  
- **Web, Government, and Healthcare** sectors are most affected.  
- A handful of **mega-breaches** (e.g., Yahoo, Facebook, LinkedIn) account for the majority of records lost.  
- Breach incidents surged after **2018**, reflecting greater digital exposure and cloud dependence.  

---

## 📊 Visualizations

> Recommended visuals for GitHub or poster inclusion:
- 📈 *Breach Count Over Time* (line chart)  
- 🧭 *Top Sectors by Number of Breaches* (bar chart)  
- 🔒 *Breach Methods Distribution* (pie chart)  
- 💥 *Top 10 Largest Breaches by Records Lost* (table)

*(Include images in a `/visuals` folder and embed them here, e.g. `![chart](./visuals/breach_trends.png)`)*

---

## 🧩 Limitations & Next Steps

### ⚠️ Limitations
- Dataset underrepresents unreported or small-scale breaches.  
- Inconsistent reporting across countries.  
- No direct measure of financial loss or breach duration.

### 🚀 Next Steps
- Apply **machine learning anomaly detection** to forecast breach risks.  
- Integrate **real-time SIEM data** (e.g., Wazuh or TheHive).  
- Build an interactive **dashboard using Plotly or Streamlit**.

---

## 👨‍💻 Author

**Name:** Maverick Walker  
**Project Track:** Data Science  
**Major:** Cybersecurity & Data Analytics  

🔗 **Connect with Me:**  
- [LinkedIn](https://www.linkedin.com/)  
- [GitHub](https://github.com/)  
- [Email](mailto:youremail@example.com)  

---

## 🏁 Acknowledgements
Special thanks to:
- The **Big Data & Analytics Association (BDAA)** for the project framework  
- The **Balloon Race Data Breach Dataset** maintainers for open data access  
- The global cybersecurity research community promoting transparency and awareness

---

## 📦 Repository Structure

📂 data_breach_analysis/
├── data/
│ └── breaches.csv
├── notebooks/
│ └── data_breach_analysis.ipynb
├── visuals/
│ ├── breach_trends.png
│ ├── top_sectors.png
│ ├── breach_methods.png
│ └── largest_breaches.png
├── README.md
└── requirements.txt


---

## 📸 Poster Preview

> This project aligns with the **BDAA Project Poster** format:
> - Problem Statement  
> - Methodology  
> - EDA Summary  
> - Results & Insights  
> - Acknowledgements & QR Code  
> 
> *(Include your final poster image here once completed — e.g., `poster.png`)*

---

## 🧾 License
This project is released under the **MIT License** — free for educational and portfolio use.

---

**Last Updated:** October 2025
