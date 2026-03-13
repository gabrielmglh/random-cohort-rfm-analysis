# 📊 Customer Cohort Analysis and RFM Segmentation

A cohort analysis is widely used to understand how specific groups behave overtime. Instead of looking at all users as a single unit, you break them into related groups (cohorts) to see if their behavior improves or declines. 

Another useful technique is the RFM (Recency, Frequency, Monetary) analysis. This technique use these three parameters to categorize customers and rate them (usually in a scale of 1 to 5). Then segments are created with respect to these rates.

These two techniques combined can provide a strong background to build strategies to retain or acquire more customers overtime. In this project, I generate a random dateset using the Numpy library and then apply these data analysis techniques using the Pandas, Matplotlib and Seaborn libraries to extract relavant informations of this data. 

---

## 📈 Objectives

The goal of this project is to analyze customer purchasing behavior and answer questions such as:

- How well does the company retain customers over time?
- What proportion of customers become loyal buyers?
  
---

## 🔬 Techniques Used

### Cohort Analysis

Customers are grouped by the month of their first purchase. Then we measure how many customers return in subsequent months. This produces a retention matrix, visualized using a heatmap.

### RFM Segmentation

RFM is a marketing technique based on three metrics:

| Metric | Description |
|------|------|
| **Recency** | How recently the customer made a purchase |
| **Frequency** | How often the customer purchases |
| **Monetary** | How much the customer spends |

Customers are scored and grouped into segments such as:

- Top value
- Very high value
- High value
- Mid value
- Low value

These segments help businesses design targeted marketing strategies.

---

## 📊 Visualizations

The project includes two visualizations:

### Cohort Retention Heatmap
Shows customer retention across time.

### RFM Segment Distribution
Displays the number of customers in each segment.

---

## 🛠 Technologies Used

- Python
- pandas
- numpy
- matplotlib
- seaborn
- Jupyter Notebook

---
## 🖼️ Results 

The analysis produced the following visualizations.

### Cohort Analysis

The heatmap below shows the retention matrix obtained from the cohort analysis.  Each row represents a cohort of customers grouped by the month of their first purchase, while each column represents the number of months since acquisition.

<p align="center">
  <img src="/graphs/cohort_analysis.png" width="80%">
</p>

### RFM segmentation

The following chart displays the distribution of customers across the RFM segments.  It provides a quick overview of how customers are classified according to their purchasing behavior.

<p align="center">
  <img src="/graphs/segment_distribution.png" width="80%">
</p>

---

## 💡 Insights 

Since the dataset used in this project was randomly generated, it does not reflect realistic customer behavior over time. Therefore, the patterns observed in the visualizations should be interpreted only as a demonstration of the analytical workflow rather than meaningful business insights.

The purpose of this project is to demonstrate how cohort analysis and RFM segmentation can be implemented in Python, including data preparation, transformation, and visualization.

As a next step, this methodology could be applied to real-world datasets in order to extract insights about customer retention and purchasing patterns. For example, a suitable dataset for this type of analysis is the [Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce).

---

## 🧠 Challenges and Learning

During the development of this project, the following skills were practiced:

- Generating sample datasets using NumPy
- Data manipulation and transformation using Pandas
- Handling missing values and restructuring data for analysis
- Building retention matrices for cohort analysis
- Implementing RFM segmentation logic
- Creating clear visualizations using Matplotlib and Seaborn

---

## ▶️ How to Run the Project

Clone the repository:

```bash
git clone https://github.com/gabrielmglh/random-cohort-rfm-analysis.git

```
Create a virtual environment 

```bash
python -m venv .venv
```

Activate the environment for Linux/Mac

```bash
source .venv/bin/activate
```
or for Windows 
```bash
venv\Scripts\activate
```

Install dependencies 

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

Run the notebook

```bash
jupyter notebook
```
