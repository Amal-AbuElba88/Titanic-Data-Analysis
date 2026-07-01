# Titanic Dataset - Exploratory Data Analysis 🚢📊

This repository contains a comprehensive Exploratory Data Analysis (EDA) on the famous Titanic dataset. The project focuses on handling missing real-world data, engineering insights through statistical grouping, and discovering the core demographic socio-economic factors that influenced passenger survival rates.

---

## 📌 Core Analysis Workflow

### 1. Data Assessment & Profiling
* **Source:** Classic Titanic Training Dataset (`train.csv`)[cite: 3].
* Utilized Pandas functions (`.head()`, `.info()`, and `.describe()`) to understand structural data types, boundary constraints, and preliminary summary statistics[cite: 3].

### 2. Strategic Data Imputation (Handling Missing Values)
Addressed significant missing data gaps to prevent model and analytical distortion:
* **Age Column:** Imputed missing entries using the dataset's **Median** age to reduce outlier skewness[cite: 3].
* **Embarked Column:** Filled gaps with the **Mode** (most frequent port of embarkation)[cite: 3].
* **Cabin Column:** Captured high-cardinality missing data by replacing null entries with a structural `"Unknown"` string label[cite: 3].

### 3. Advanced Data Aggregation & Reshaping
Leveraged Pandas execution power to slice the data across multiple dimensions:
* Computed multi-level demographic metrics using `.groupby()` to isolate average age and fare distributions across genders and ticket classes[cite: 3].
* Reshaped data arrays using `.unstack()` to build cross-tabulation matrices analyzing relational survival probabilities[cite: 3].

### 4. Data Visualization (`matplotlib`)
Generated clean graphical plots to visualize correlation and distribution patterns:
* **Gender vs. Survival:** Bar charts illustrating that female passengers had a significantly higher survival frequency[cite: 3].
* **Socio-Economic Class vs. Survival:** Analyzed how Pclass (Ticket Class) directly affected survival, revealing a strong survival bias toward 1st-class passengers[cite: 3].
* **Age Distribution:** Histograms capturing the comprehensive distribution of passenger ages[cite: 3].
* **Correlation Mapping:** Created visual **Heatmaps** via `imshow()` to render multi-dimensional survival rates intuitively[cite: 3].

---

## 💡 Key Learnings & Insights
* **Demographics Matter:** Gender was an extreme driver for survival, validating the historical "women and children first" protocols[cite: 3].
* **Socio-Economic Privilege:** Ticket class had a massive correlation with survival rates, indicating better access to lifeboats for upper-class passengers[cite: 3].

---

## 📄 Project Context & Outputs
* **Institution:** University College of Applied Sciences (UCAS)[cite: 3]
* **Supervision:** Dr. Ahmed Al Dahdoh[cite: 3]
* **Developer:** Amal Ahmed Abu Elba[cite: 3]
* **Student ID:** 220231850[cite: 3]
* **Project Report:** Full analysis available in [`Titanic Dataset Analysis Report.pdf`](./Titanic%20Dataset%20Analysis%20Report.pdf)
