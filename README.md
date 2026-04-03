# MedRx Pharmacy Sales Analysis Dashboard

![Dashboard Preview](assets/Sales_Intelligence.png)

## Overview

A comprehensive Power BI pharmacy sales analytics solution for **MedRx**, covering revenue performance, product insights, regional analysis, and sales rep performance across Nigeria.

The project spans **January 2024 – May 2025** and tracks 8 drugs across 4 drug categories, 4 Nigerian regions, and 5 sales representatives.

---

## Dashboard Views

### 1. Sales Intelligence
> Monthly trends, regional revenue, rep performance, and category breakdowns.

![Sales Intelligence](assets/Sales_Intelligence.png)

### 2. Market Pulse
> Top-selling drugs, revenue vs profit scatter, and seasonal drug demand patterns.

![Market Pulse](assets/Market_Pulse.png)

---

## Key Metrics (2024)

| Metric | Value | vs Prior Year |
|---|---|---|
| Revenue | $3,613,765 | ▼ 56.6% |
| Units Sold | 55,987 | ▼ 58.2% |
| Profit | $272,872 | ▼ 57.3% |
| Profit Margin | 8% | ▼ 52.4% |

---

## Data Model

### Source File
`data/Pharmacy_Sales_Analysis.xlsx`

### Sheets
| Sheet | Description |
|---|---|
| `Raw_Data` | Original transaction records |
| `Clean_Data` | Processed data used for analysis |
| `Pivot_Analysis` | Pre-aggregated pivot tables |
| `Sales Intelligence` | Dashboard sheet 1 |
| `Market Pulse` | Dashboard sheet 2 |

### Key Fields (Clean_Data)

| Column | Type | Description |
|---|---|---|
| `Date` | Date | Transaction date |
| `Region` | Text | Nigerian region (Eastern, Western, Northern, Southern) |
| `Drug_Name` | Text | Drug product name |
| `Category` | Text | Drug category (Antibiotic, Cardiovascular, Diabetes Care, Pain Relief) |
| `Sales_Rep` | Text | Sales representative name |
| `Units_Sold` | Integer | Number of units sold |
| `Unit_Price` | Float | Price per unit (USD) |
| `Revenue` | Float | Total revenue |
| `Cost` | Float | Total cost |
| `Profit` | Float | Revenue minus Cost |
| `Profit_Margin` | Float | Profit / Revenue |

---

## Product Catalogue

| Drug | Category |
|---|---|
| Heartzol | Cardiovascular |
| Maxilin | Antibiotic |
| Glucorin | Diabetes Care |
| Relipain | Pain Relief |
| CardioVex | Cardiovascular |
| Zymetra | Antibiotic |
| Diafast | Diabetes Care |
| Neuroflex | Pain Relief |

---

## Regional Coverage

- **Eastern Nigeria**
- **Western Nigeria**
- **Northern Nigeria**
- **Southern Nigeria**

---

## Sales Team

| Rep | Region Focus |
|---|---|
| Emeka Obi | Multi-region |
| Grace Umeh | Multi-region |
| Jane Akins | Multi-region |
| Laila Hussein | Multi-region |
| Mohammed Bello | Multi-region |

---

## Project Structure

```
medrx-pharmacy-dashboard/
│
├── data/
│   └── Pharmacy_Sales_Analysis.xlsx    # Master data file with all sheets
│
├── assets/
│   ├── Sales_Intelligence.png          # Dashboard screenshot – Sales Intelligence view
│   └── Market_Pulse.png                # Dashboard screenshot – Market Pulse view
│
├── notebooks/
│   └── eda.ipynb                       # Exploratory data analysis notebook
│
├── src/
│   ├── clean_data.py                   # Data cleaning & preprocessing script
│   └── analysis.py                     # Summary statistics & aggregation helpers
│
├── docs/
│   └── data_dictionary.md              # Field-level documentation
│
└── README.md
```

---

## Getting Started

### Prerequisites
- Python 3.8+
- pandas, openpyxl, matplotlib, seaborn

### Installation

```bash
git clone https://github.com/your-username/medrx-pharmacy-dashboard.git
cd medrx-pharmacy-dashboard
pip install -r requirements.txt
```

### Run Analysis

```bash
python src/analysis.py
```

### Open Notebook

```bash
jupyter notebook notebooks/eda.ipynb
```

---

## Power BI Setup

1. Open Power BI Desktop
2. **Get Data → Excel** → select `data/Pharmacy_Sales_Analysis.xlsx`
3. Load the `Clean_Data` sheet
4. Refresh relationships and validate DAX measures
5. Dashboard pages: **Sales Intelligence** and **Market Pulse**

---

## License

MIT License — see [LICENSE](LICENSE) for details.

---

*Built with Microsoft Power BI | Data: MedRx Internal Sales Records*
