# 🏙️ Airbnb Paris Price Analysis

This project explores **factors that influence Airbnb prices in Paris**, using data from [Inside Airbnb](https://insideairbnb.com/get-the-data/).  
It aims to identify what drives listing prices — location, host characteristics, availability, and more — through statistical and visual analysis.

---

## 🧾 Data Overview
### 🗂️ Raw Data (Before Preprocessing)
- Source: Inside Airbnb – Paris Listings
- Shape: 84,055 rows × 79 columns
- Description:
The raw dataset included extensive details about listings, hosts, and reviews — such as URLs, descriptions, coordinates, amenities, host profile details, and calendar data.

After cleaning and preprocessing, variables were selected for regression modeling to explain the **log-transformed price** (`log(price)`).

---

## 🧠 Objectives
1. Identify **key drivers of Airbnb pricing** in Paris  
2. Visualize and understand **distribution of review scores, host characteristics, and location patterns**  
3. Apply **OLS regression** to quantify each variable’s impact on price  
4. Extract **business insights** for hosts and platform operators

---

## 🧩 Key Analysis Steps
- **Data Cleaning:** handled missing values, outliers, and encoded categorical variables  
- **EDA (Exploratory Data Analysis):** visualized price distribution, room types, and review score patterns  
- **Regression Modeling:**  
  - Dependent variable: `log(price)`  
  - Robust standard errors (HC3) applied  
  - Checked model assumptions and multicollinearity (VIF, condition number)

---

## 📈 Main Findings
- **Tourism districts** (Louvre, Opéra, etc.) enjoy a ~23% price premium  
- **Superhosts** and experienced hosts charge higher rates (+3–6%)  
- **Entire homes** and **hotel-type rooms** command strong premiums, while shared rooms are ~50% cheaper  
- **Minimum stay length** negatively affects price (short-term flexibility = higher demand)  
- Review scores are highly concentrated (4.7–5.0 range), showing **limited variance and high multicollinearity**

---

## 💡 Business Insights
- **Location premium** remains dominant — proximity to tourist attractions significantly boosts price  
- **Reputation matters** — Superhosts benefit from trust-based price advantages  
- **Flexibility pays off** — shorter minimum stays attract higher willingness to pay  
- **User convenience** — instant booking availability correlates with higher prices  

---

## 🧰 Tech Stack
- **Language:** Python  
- **Libraries:** pandas, numpy, seaborn, matplotlib, statsmodels  
- **Environment:** Jupyter Notebook (.ipynb)

---

## 📬 Notes
This project is for academic and educational purposes only.  