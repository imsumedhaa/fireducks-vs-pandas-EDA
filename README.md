# fireducks-vs-pandas-EDA
This repo benchmarks and compares Exploratory Data Analysis (EDA) and Data Visualization workflows using FireDucks and Pandas on large datasets. It demonstrates performance differences in filtering, grouping, sorting, and reading data—highlighting FireDucks as a blazing-fast alternative for modern data science pipelines.
# 🔥 EDA & Visualization: FireDucks vs Pandas

This project benchmarks **FireDucks** against **Pandas** for Exploratory Data Analysis on large datasets.

## 📌 Introduction
Exploratory Data Analysis (EDA) is crucial for understanding data patterns. However, Pandas can slow down with datasets exceeding 10M+ rows. Enter **FireDucks** — a blazing-fast, drop-in Pandas alternative.

## 🎯 Problem
Traditional tools like Pandas struggle with performance and memory when handling massive datasets.

## ✅ Approach
- Create synthetic sales data (10M rows)
- Benchmark: Load, Filter, GroupBy, Visualize
- Compare execution times between Pandas and FireDucks

## 🛠️ Tools
- Python 3.8+
- Pandas
- FireDucks
- NumPy
- Matplotlib

## 🧪 Sample Benchmark (10M rows)

| Task                   | Pandas Time (s) | FireDucks Time (s) |
|------------------------|------------------|---------------------|
| Load CSV               | 18.4             | 4.3                 |
| Filter price > 100     | 3.2              | 1.1                 |
| GroupBy avg by region  | 1.9              | 0.5                 |
| Summary Stats          | 2.6              | 0.7                 |

## 📊 Visualization

Both tools use Matplotlib for grouped bar charts comparing average units sold by region.

## ⚡ Enable Benchmark Mode
```python
import fireducks.pandas as fd
fd.set_mode("benchmark")
