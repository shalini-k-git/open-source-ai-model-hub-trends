# 🌐 AI Model Ecosystem Analysis

## 📌 Project Overview

The AI model ecosystem is expanding rapidly, yet adoption remains highly unequal.  
This project analyzes 550 AI models from the Hugging Face platform to understand the structural and growth dynamics that drive model popularity.

The study combines cross-sectional model analysis and time-series growth tracking to evaluate performance inequality, lifecycle momentum, and ecosystem behavior.

---

## 🎯 Problem Statement

Despite the rapid growth of open-source AI models, adoption is heavily concentrated among a small number of models.

This project aims to:

- Identify structural inequalities in model downloads  
- Analyze lifecycle-based growth momentum  
- Compare company-developed vs individual models  
- Examine geographic performance differences  
- Evaluate whether the ecosystem follows a heavy-tailed distribution  

---

## 📂 Dataset Description

- **550 Unique AI Models**
- Weekly cumulative download tracking
- Panel data structure (same models observed weekly)

### Metadata Includes:

- Model Name  
- Author  
- Organization Type  
- Country  
- Modality (Unimodal / Multimodal)  
- Supported Languages  
- Download Counts  
- Annotator Count  
- Access Tier  

### Data Structure Design

Because downloads are cumulative and tracked weekly:

- Latest observation per model → used for static performance analysis  
- Full weekly history → used for growth and volatility analysis  

---

## 🛠 Methodology

### 1️⃣ Data Cleaning
- Standardized column names  
- Converted date formats  
- Parsed list-type columns using `ast.literal_eval`  
- Handled missing and uncertain values  
- Ensured consistent datatype alignment  

### 2️⃣ Feature Engineering

#### Static (Model-Level) Features
- `has_known_lineage`
- `same_author_derived`
- `is_multimodal_input`
- `is_active_model`

#### Time-Series Features
- `model_age_days`
- `model_age_weeks`
- `weekly_growth`
- `rolling_4week_growth`
- `acceleration`
- `model_stage` (Launch, Early Growth, Growth, Mature)

---

## 📊 Exploratory Data Analysis

### Univariate Analysis
- Download distribution (Histogram + KDE)
- Organization type distribution
- Modality distribution
- Lifecycle stage distribution

### Bivariate Analysis
- Downloads vs Organization Type
- Downloads vs Country
- Downloads vs Modality
- Downloads vs Annotator Count

### Multivariate Analysis
- Lifecycle stage vs Growth Momentum
- Organization Type vs Lifecycle Performance
- Correlation Analysis

---

## 🔎 Key Insights

- 📈 Downloads are highly right-skewed → Winner-takes-all ecosystem  
- 🏢 Company-developed models outperform individual models at higher percentiles  
- 🌍 Certain countries dominate high-average adoption  
- 🚀 Early Growth stage models show strongest weekly momentum  
- ⚡ Launch stage models exhibit highest volatility  
- 🔬 Weak correlation between annotator count and adoption  
- 📊 High variance and kurtosis confirm heavy-tailed behavior  

---

## 💡 Strategic Recommendations

- Invest in early-growth stage models to capture momentum  
- Strengthen institutional-backed development pipelines  
- Optimize model release timing during ecosystem surge periods  
- Focus on high-demand unimodal applications  
- Prioritize differentiation over annotator volume  

---

## 🧰 Tech Stack

- Python (Pandas, NumPy)
- Matplotlib & Seaborn
- Plotly
- SQL
- Jupyter Notebook

---

## 📈 Statistical Characteristics

- High Variance → Significant inequality in model adoption  
- High Skewness → Extreme right-tail dominance  
- High Kurtosis → Presence of heavy outliers  
- Weak linear correlations → Complex growth drivers  

---

## 🚀 Future Scope

- Predictive modeling for download forecasting  
- Lifecycle survival analysis  
- Model lineage network analysis  
- Interactive dashboard deployment  

---

## 👩‍💻 Author

**Shalini Kandaswamy**  
Data Analytics | AI Ecosystem Research | Growth Analytics
