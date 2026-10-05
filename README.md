# 📊 UPI Transactions Analysis: Power BI Project

An interactive Power BI dashboard that analyses UPI transactions to understand user behavior, transaction patterns, and remaining balances, with slicers, bookmarks, and conditional formatting.

---

## 🚀 Project Overview

This project analyses UPI transactions using Power BI. The dataset was transformed, cleaned, and visualized to understand user behavior, transaction patterns, and balances. The final dashboard supports interactive filtering with slicers, bookmarks, and formatted visuals.

---

## ❓ What Can Be Analyzed?

- What spending trends can be observed from UPI transactions?
- How do age groups differ in transaction behavior?
- Which time periods show peak or low UPI usage?
- Can slicers and filters help identify specific user segments?
- How do remaining balances and transactions interact over time?

---

## 📂 Dataset Description


| Column | Description |
|---|---|
| Age Groups | Segmented age brackets (created via DAX) |
| Amount | Transaction amount in INR |
| BankNameReceived | Bank where funds were received |
| BankNameSent | Bank from which funds were sent |
| City | Customer's city of transaction |
| Currency | Currency used (mostly INR) |
| CustomerAccount | Customer's account identifier |
| CustomerAge | Age of the customer |
| DeviceType | Type of device used (Mobile, Desktop, etc.) |
| Gender | Gender of the customer |
| MerchantAccount | Merchant's account identifier |
| MerchantName | Merchant's name (e.g. Paytm, Amazon) |
| PaymentMethod | Payment method chosen (UPI ID, QR Code, etc.) |
| PaymentMode | Mode of transaction (Send/Receive) |
| Purpose | Purpose of payment (shopping, bills, etc.) |
| RemainingBalance | Balance left after the transaction |
| Status | Transaction status (Success/Failed/Pending) |
| TransactionDate | Date of the transaction |
| TransactionID | Unique ID for each transaction |
| TransactionTime | Time of the transaction |
| TransactionType | Type of UPI transaction (P2P, P2M, etc.) |

---

## 🔨 Steps I Performed

### 1. Loading Data into Power BI Desktop
- Imported the UPI transactions dataset into Power BI.

### 2. Data Profiling
- Validated data types, null values, duplicates, and overall structure.

### 3. Slicers Creation & Symmetrical Positioning
Created **10 slicers** for interactive filtering:

1. BankNameSent
2. BankNameReceived
3. City
4. DeviceType
5. Gender
6. Age Groups
7. MerchantName
8. PaymentMethod
9. Purpose
10. TransactionType

📐 Slicers are placed in two rows with equal spacing for symmetry and a better user experience.

### 4. Age Group Column (via DAX)

```DAX
Age Groups = 
IF('UPI Transactions'[CustomerAge] <= 25, "A1",
   IF('UPI Transactions'[CustomerAge] <= 35, "A2", "A3"))
```

| Group | Age Range |
|---|---|
| A1 | 25 and below |
| A2 | 26 to 35 |
| A3 | Above 35 |

### 5. Visualizations
- Line Chart: transaction trends over time
- Column Chart: balance by month
- Matrix Visual: tabular insights
- Conditional formatting to highlight key insights

### 6. Bookmarks & Enhancements
- Synced slicers across pages
- Added bookmarks for Transactions and Remaining Balance
- Enhanced slicer formatting for a cleaner UI

---

## 🖼 Screenshots

### 1. Column Chart (Transaction Amounts)
<img width="1435" height="805" alt="CCAmounts" src="https://github.com/user-attachments/assets/2b34b95f-4367-4fe1-9b4a-4743f1b3dc81" />


### 2. Column Chart (Balance Trends)
<img width="1446" height="806" alt="CCB" src="https://github.com/user-attachments/assets/0ed801d9-eaa3-42d9-a254-4bdc4f3e82a4" />


### 3. Line Chart (Balance Trends)
<img width="1432" height="807" alt="LCB" src="https://github.com/user-attachments/assets/8ff930f1-ad37-46d0-b3a1-ede193ffe4b2" />


### 4. Line Chart (Transaction Trends)
<img width="1432" height="808" alt="LineChart" src="https://github.com/user-attachments/assets/b2cbb79b-d7d4-4a69-b1e9-3c066df8203f" />


### 5. Matrix Visual (Detailed Insights)
<img width="1435" height="805" alt="MatrixVisual" src="https://github.com/user-attachments/assets/4e0c0350-39e8-47b4-a93a-84bae3674026" />


---

## ⚡ How to Use the Report

1. Download the `.pbix` file and open it in **Power BI Desktop** 
2. Use the slicers to filter transactions dynamically.
3. Use the bookmarks to switch between views.
4. (Optional) View the published version on Power BI Service: [add link if you have one]

---

## 📌 Insights & Future Enhancements

- Compare UPI transaction patterns across demographics and cities
- Add advanced DAX measures for profitability and frequency insights
- Integrate with real-time UPI datasets for live dashboards
- Use AI visuals (Q&A, Key Influencers) for deeper exploration

---

## 🛠 Tech Stack

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-0078D4?style=for-the-badge)
![Excel](https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white)

- **Tool:** Power BI Desktop
- **Language:** DAX (calculated columns and measures)
- **Data Source:** UPI Transactions dataset

---

## 👩‍💻 Author

**Aditi Sharma**
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/aditi0105/?isSelfProfile=true)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/aditis0105)
