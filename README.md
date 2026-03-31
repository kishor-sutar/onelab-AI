# 🏦 Fintech Reconciliation Engine

A structured, production-oriented reconciliation system that simulates real-world payment platform vs bank settlement mismatches using Python and pandas.

---

## 🚀 Overview

In payment systems, transactions are recorded instantly, while bank settlements occur with delays (T+1 / T+2). This project builds a reconciliation pipeline to detect discrepancies between the two systems.

---

## ⚙️ Features

- Synthetic dataset generation (platform + bank)
- Realistic anomaly injection:
  - Late settlements (month spillover)
  - Rounding differences
  - Duplicate bank entries
  - Refunds without original transactions
- Full reconciliation using `txn_id`
- Detection of:
  - Missing settlements
  - Unexpected bank entries
  - Amount mismatches
  - Duplicate records
  - Late settlements
- Transaction-level correction logic (avoids duplicate inflation)
- Validation checks for correctness

---

## 🧠 Key Insight

Reconciliation is not just about joins — it's about:
- **Data integrity**
- **Temporal correctness**
- **Handling duplicates properly**

This project demonstrates how naive row-level logic can produce misleading results and how to fix it using transaction-level aggregation.

---

## 📊 Tech Stack

- Python
- pandas
- NumPy
- Jupyter Notebook

---

## 📁 Structure



---

## ✅ How to Run

1. Clone the repository  
2. Open the notebook in Jupyter  
3. Run cells sequentially  

---

## 📌 Output

Final report includes:
- Count of discrepancies
- Detailed breakdown tables
- Validation checks

---

## 💡 Author

Kishor Sutar   

---

## 🔥 Note

This project is designed to reflect **real fintech reconciliation challenges**, not toy examples.