# StreamingEvents-MarketingInsights 📺📊

A comprehensive data analysis project examining streaming platform user behavior, content performance, and marketing effectiveness using a synthetic dataset of 50,501 content events.

## 📋 Table of Contents

- [🎯 Project Overview](#-project-overview)
- [📊 Dataset Description](#-dataset-description)
  - [User Demographics](#user-demographics)
  - [Content Information](#content-information)
  - [Engagement Metrics](#engagement-metrics)
  - [Marketing & Revenue](#marketing--revenue)
- [🏗️ Project Structure](#️-project-structure)
- [🛠️ Setup and Installation](#️-setup-and-installation)
  - [Prerequisites](#prerequisites)
  - [Installation Steps](#installation-steps)
  - [Option A: Using Python venv (Standard)](#option-a-using-python-venv-standard)
  - [Option B: Using Conda/Miniconda (Recommended for Data Science)](#option-b-using-condaminiconda-recommended-for-data-science)
  - [Reactivating Your Environment](#reactivating-your-environment)
- [🔍 Analysis Workflow](#-analysis-workflow)
  - [Phase 1: Data Exploration & Cleaning](#phase-1-data-exploration--cleaning)
  - [Phase 2: User Behavior Analysis](#phase-2-user-behavior-analysis)
  - [Phase 3: Content Performance Analysis](#phase-3-content-performance-analysis)
  - [Phase 4: Marketing Effectiveness](#phase-4-marketing-effectiveness)
  - [Phase 5: Revenue Optimization](#phase-5-revenue-optimization)
- [📈 Key Technologies](#-key-technologies)
  - [Data Science & Analytics](#data-science--analytics)
  - [Development Environment](#development-environment)
  - [Data Visualization](#data-visualization)
- [🎯 Key Research Questions](#-key-research-questions)
  - [1. Binge-Watching Behavior & Churn Risk Analysis](#1-binge-watching-behavior--churn-risk-analysis)
  - [2. Ad Performance & Geographic Conversion Analysis](#2-ad-performance--geographic-conversion-analysis)
  - [3. Platform-Genre Ad Inventory Optimization](#3-platform-genre-ad-inventory-optimization)
- [📊 Expected Deliverables](#-expected-deliverables)
  - [📁 GitHub Repository](#-github-repository)
  - [🧹 Cleaned & Processed Data](#-cleaned--processed-data)
  - [📓 Jupyter Notebooks](#-jupyter-notebooks)
  - [📋 Written Insights Reports](#-written-insights-reports)
  - [📊 Dashboard](#-dashboard)
  - [🎤 Slide Deck](#-slide-deck)
  - [🔧 Supplementary Files](#-supplementary-files)
- [🔬 Methodology & Standards](#-methodology--standards)
- [📄 Project Purpose](#-project-purpose)
- [🟢 Current Progress](#-current-progress)

## 🎯 Project Overview

This project analyzes streaming platform data to uncover insights about:
- **User Engagement Patterns**: Watch time, completion rates, and binge-watching behavior
- **Content Performance**: Popular genres, content types, and viewer preferences
- **Marketing Effectiveness**: Channel performance, ad engagement, and conversion rates
- **Revenue Optimization**: ECPM analysis, subscription types, and monetization strategies
- **Churn Analysis**: Risk factors and user retention patterns

## 📊 Dataset Description

The raw dataset (`content_events_50k_raw.csv`) contains **50,501 streaming events** with the following key attributes:

### User Demographics
- User ID, age group, gender, country
- Account creation date, churn risk score
- Subscription type and returning user status

### Content Information
- Content ID, type (Movie/Episode/News), title, genre
- Release date, episode number, duration
- User ratings and completion percentages

### Engagement Metrics
- Watch duration, percent completed, buffer counts
- Device type, platform, viewing mode
- Binge session indicators, exit reasons

### Marketing & Revenue
- Marketing channels, ad exposure, impressions/clicks
- ECPM, revenue, margins, conversion data
- Fill rates and data source tracking

## 🏗️ Project Structure

```
StreamingEvents-MarketingInsights/
├── data/
│   ├── raw/                     # Original dataset
│   │   └── content_events_50k_raw.csv
│   └── processed/               # Cleaned and aggregated data
├── notebooks/                   # Jupyter notebooks for analysis
│   └── 01_data_quality_audit.ipynb  # Data quality exploration & issue logging
├── sql/                         # SQL queries and database files
├── dashboard/                   # Interactive dashboards
├── reports/                     # Final analysis reports
│   └── 01_data_issues_log.csv   # Automated data quality issues tracking
├── slides/                      # Presentation materials
├── requirements.txt             # Python dependencies
└── README.md                    # Project documentation
```

## 🛠️ Setup and Installation

### Prerequisites
- Python 3.8+ (or Miniconda/Anaconda)
- Jupyter Lab/Notebook
- Git

### Installation Steps

Choose one of the following approaches:

#### Option A: Using Python venv (Standard)

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd StreamingEvents-MarketingInsights
   ```

2. **Create a virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\\Scripts\\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Launch Jupyter Lab**
   ```bash
   jupyter lab
   ```

#### Option B: Using Conda/Miniconda (Recommended for Data Science)

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd StreamingEvents-MarketingInsights
   ```

2. **Create a conda environment**
   ```bash
   conda create -n marketinganalysis python=3.12
   conda activate marketinganalysis
   ```

3. **Install dependencies with pip**
   ```bash
   pip install -r requirements.txt
   ```
   
   *Note: We use pip inside the conda environment to ensure exact version compatibility with the requirements.txt file.*

4. **Launch Jupyter Lab**
   ```bash
   jupyter lab
   ```

5. **To deactivate the environment when done**
   ```bash
   conda deactivate
   ```

#### Reactivating Your Environment

For future sessions:
- **venv users**: `source venv/bin/activate` (or `venv\\Scripts\\activate` on Windows)
- **conda users**: `conda activate marketinganalysis`

### Setting Up Jupyter Kernel in VS Code

To use your environment in VS Code notebooks:

1. **Register the environment** (run once in your activated environment):
   ```bash
   python -m ipykernel install --user --name marketinganalysis --display-name "Python (marketinganalysis)"
   ```

2. **In VS Code**: Reload window (`Ctrl+Shift+P` → "Reload Window"), open a notebook, and select **Python (marketinganalysis)** from the kernel picker.

## 🔍 Analysis Workflow

### Phase 1: Data Quality Audit & Issue Resolution
- Comprehensive data quality exploration and conceptualization
- Automated issue logging across all data dimensions
- Issue resolution strategy development
- Purpose-driven cleaning decisions based on analytical objectives

### Phase 2: Data Cleaning & Processing
- Implementation of validated issue resolutions
- Purpose-driven data cleaning based on analytical needs
- Clean dataset export in optimized format
- Data validation and quality assurance

### Phase 3: User Behavior Analysis
- Demographic segmentation
- Engagement pattern analysis
- Churn risk modeling
- User journey mapping

### Phase 4: Content Performance Analysis
- Genre popularity trends
- Content completion rates
- Seasonal viewing patterns
- Device and platform preferences

### Phase 5: Marketing Effectiveness
- Channel attribution analysis
- Ad engagement metrics
- Conversion funnel analysis
- ROI calculations by channel

### Phase 6: Revenue Optimization
- ECPM analysis by segment
- Subscription type performance
- Revenue per user calculations
- Margin optimization opportunities

## 📈 Key Technologies

### Data Science & Analytics
- **pandas** - Data manipulation and analysis
- **numpy** - Scientific computing
- **matplotlib & seaborn** - Static visualizations
- **plotly** - Interactive visualizations
- **scikit-learn** - Machine learning algorithms
- **scipy** - Statistical analysis
- **tabulate** - Formatted table output for data quality reporting

### Development Environment
- **Jupyter Lab** - Interactive development
- **IPython** - Enhanced Python shell
- **Git** - Version control

### Data Visualization
- **Tableau** - Business intelligence dashboards
- **Power BI** - Executive reporting
- **Plotly Dash** - Web-based analytics apps

## 🎯 Key Research Questions

### 1. Binge-Watching Behavior & Churn Risk Analysis
**How do binge-watching patterns (session count, total watch time) vary by age group and subscription tier—and how are they correlated with churn risk?**

**Business Impact:**
- **Retention Marketing**: Target binge-friendly features to high-value, low-churn segments
- **Customer Lifetime Value**: Optimize acquisition campaigns for demographic segments with favorable binge-to-retention ratios
- **Personalized Campaigns**: Deploy targeted retention strategies for high-risk binge-watchers

**Key Metrics:**
- Binge sessions per user by `AGE_GROUP` × `SUBSCRIPTION_TYPE`
- Total binge minutes vs `CHURN_RISK_SCORE` correlation
- Cohort analysis: "% of binge-watchers still active at 30/60/90 days"

### 2. Ad Performance & Geographic Conversion Analysis
**How does ad performance (impressions, click-through rates, eCPM) vary by subscription tier and country—and what is the resulting ecommerce conversion impact?**

**Business Impact:**
- **Ad Revenue Optimization**: Identify high-performing platform/geo combinations for budget reallocation
- **Geo-Targeted Campaigns**: Customize creatives and landing pages based on regional performance patterns
- **Subscription Upsell**: Leverage ad engagement data to identify conversion opportunities

**Key Metrics:**
- CTR (`AD_CLICKS` / `AD_IMPRESSIONS`) by `SUBSCRIPTION_TYPE` × `COUNTRY_CODE`
- eCPM analysis across geographic and subscription segments
- Conversion funnel: Impressions → Clicks → `ECOMMERCE_CONVERSION`

### 3. Platform-Genre Ad Inventory Optimization
**Which platforms and content genres exhibit low ad fill-rate and low CPM, and how does that impact total ad revenue and margin?**

**Business Impact:**
- **Ad Ops Efficiency**: Identify underperforming inventory for SSP optimization or floor price adjustments
- **Platform-Genre Investment**: Guide content promotion and exclusive rights negotiations
- **Margin Optimization**: Reallocate resources from low-margin to high-margin inventory segments

**Key Metrics:**
- `FILL_RATE` × `ECPM_USD` analysis by `PLATFORM` × `GENRE` combinations
- Total `REVENUE_USD` and `MARGIN_USD` contribution by segment
- Identification of underperforming cells (fill rate < 60% or eCPM < $5)

## 📊 Expected Deliverables

### 📁 GitHub Repository
- Well-structured folder layout (`data/`, `notebooks/`, `dashboard/`, `reports/`, `slides/`, `sql/`)
- Clear README.md explaining project objectives, reproduction steps, and links to key artifacts
- Version-controlled analysis with reproducible methodology

### 🧹 Cleaned & Processed Data
- **Master Dataset**: `data/processed/clean_content_events_50k.parquet` (or SQLite DB) — cleaned dataset with proper dtypes and churn proxy
- **Aggregated Analysis Files** in `data/processed/`:
  - `users_binge.csv` — binge-session and churn metrics per user
  - `ad_summary.csv` — impressions, clicks, CTR, eCPM, conversion rates by subscription & country
  - `pf_genre.csv` — fill-rate, eCPM, revenue, margin by platform & genre

### 📓 Jupyter Notebooks
- **`01_data_quality_audit.ipynb`**: ✅ **COMPLETED** - Data quality exploration, conceptualization, and automated issue logging
- **`02_data_cleaning_solutions.ipynb`**: Implementation of data cleaning based on finalized issue resolutions
- **`03_binge_churn_analysis.ipynb`**: Binge behavior → churn analysis, with 2–3 key visuals
- **`04_ad_performance_analysis.ipynb`**: Ad performance by tier & geography, with funnel and heatmap
- **`05_fillrate_cpm_analysis.ipynb`**: Platform×genre fill-rate & eCPM analysis, with bubble chart and margin summary

### 📋 Written Insights Reports (in `/reports/`)
- **`01_data_issues_log.csv`**: ✅ **COMPLETED** - Automated data quality assessment with 24 identified issues across single-column and cross-field validations
- **`02_data_issues_resolution_plan.md`**: Issue-by-issue resolution strategies and cleaning decisions
- **`00_data_dictionary.md`**: Column definitions, data types, and missingness notes
- **`03_binge_churn_insights.md`**: Methodology, charts, and marketing recommendations for Question 1
- **`04_ad_performance_insights.md`**: Methodology, charts, and recommendations for Question 2
- **`05_fillrate_cpm_insights.md`**: Methodology, visuals, and action items for Question 3
- **`Final_Marketing_Report.pdf`**: Cohesive 10–15 page executive report tying all three questions together with combined recommendations and roadmap

### 📊 Dashboard (in `/dashboard/`)
- **Tableau Workbook** (`.twbx`) or **Power BI File** (`.pbix`) showing interactive views for each question:
  - Binge & churn correlation charts
  - Ad performance funnel and eCPM bar/heatmap
  - Fill-rate vs. eCPM bubble chart and underperforming inventory table
- **Optional**: Plotly Dash or Streamlit app code for Python-based interactive dashboard
- **`dashboard/README.md`**: Instructions for loading and exploring the dashboard

### 🎤 Slide Deck (in `/slides/`)
- **`Marketing_Insights_Presentation.pptx`**: 5–7 slide executive presentation covering:
  - Project objective & context
  - Key questions & top-level KPIs
  - Binge & churn insights
  - Ad funnel & ROI insights
  - Fill-rate/CPM recommendations
  - Combined 90-day marketing roadmap

### 🔧 Supplementary Files
- **`requirements.txt`**: Python environment dependencies
- **SQL scripts**: Database queries and aggregation logic (if using SQLite)
- **Data validation scripts**: Quality assurance and testing code

---

**Portfolio Impact**: These artifacts form a complete, end-to-end marketing analytics portfolio demonstrating expertise in data ingestion, cleaning, analysis, visualization, and business communication — from raw data to executive-ready insights.

## 🔬 Methodology & Standards

This portfolio project demonstrates professional data science best practices:
- **Reproducible Analysis**: Clear documentation and version-controlled workflows
- **Data Quality**: Comprehensive cleaning, validation, and transformation processes
- **Statistical Rigor**: Appropriate methodologies with documented assumptions and limitations
- **Business Focus**: Analysis directly tied to actionable business recommendations
- **Ethical Standards**: Responsible handling of synthetic data with privacy considerations

## 📄 Project Purpose

This is a **portfolio project** designed to showcase data science and marketing analytics capabilities. The synthetic dataset enables comprehensive analysis without privacy concerns while demonstrating real-world analytical skills applicable to streaming media and digital marketing domains.

---

**Last Updated**: June 2025  
**Status**: Phase 1 Complete - Data quality audit finished. Proceeding to issue resolution planning.  
**Data Volume**: 50,501 streaming events  
**Analysis Timeframe**: Multi-year historical data (2017-2024)

## 🟢 Current Progress

### Phase 1: Data Quality Audit (COMPLETED ✅)
- ✅ **Data Conceptualization**: Established grain, key metrics, dimensions, and example record stories
- ✅ **Comprehensive Issue Logging**: Automated detection of 24 data quality issues using pandas
  - Single-column checks: null values, data types, format validation, range validation, categorical validation
  - Cross-field checks: temporal ordering, duration consistency, ads-specific rules, ID matching
- ✅ **Quality Assessment Framework**: Established systematic approach for future data validation
- ✅ **Raw Data Analysis**: Complete examination of `content_events_50k_raw.csv`

### 🔄 Current Phase: Issue Resolution Planning
- **Issue Prioritization**: Determine which issues are truly solvable vs. documentable
- **Resolution Strategy Development**: Define specific solutions for each resolvable issue
- **Impact Assessment**: Evaluate how each issue affects the three key research questions
- **Documentation Planning**: Establish guidelines for flagging and documenting persistent issues

### 📋 Next Steps
1. **Finalize Issues Log**: Complete resolution planning for all 24 identified issues
2. **Implement Data Cleaning**: Apply validated solutions in systematic cleaning process
3. **Export Clean Dataset**: Create processed data in optimal format (Parquet/SQLite)
4. **Begin Analysis Framework**: Set up notebooks for specific research questions
5. **Start Phase 2**: User behavior and binge-watching analysis

### 🔍 Data Quality Methodology

This project follows a **purpose-driven data quality approach**:
- **Deliberate Assessment**: Manual examination before automated fixes to avoid bias
- **Question-Focused Cleaning**: Only address issues relevant to analytical objectives
- **Comprehensive Logging**: Document all issues for future reference and transparency
- **Conservative Treatment**: Preserve data integrity by avoiding unnecessary modifications
- **Strategic Documentation**: Flag persistent issues with analysis considerations rather than dropping valuable data
