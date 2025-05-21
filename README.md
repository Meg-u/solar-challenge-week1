# solar-challenge-week1

## 📦 Environment Setup and final read me

```bash
# Clone the repo
git clone https://github.com/Meg-u>/solar-challenge-week1.git
cd solar-challenge-week1

# Create and activate virtual environment
python -m venv venv
source venv/bin/activate  # or .\venv\Scripts\Activate.ps1 on Windows

# Install dependencies
pip install -r requirements.txt


---

Objectives

- Clean and prepare solar datasets for analysis.
- Perform country-specific EDA for Benin, Sierra Leone, and Togo.
- Conduct cross-country statistical comparisons.
- Develop an interactive dashboard for real-time exploration of solar metrics.

---

Exploratory Data Analysis (EDA)

Each country’s dataset was cleaned and analyzed in a dedicated Jupyter notebook:

- **Benin:** Identified trends in GHI, DNI, and DHI values and seasonal patterns.
- **Sierra Leone:** Addressed significant missing values and analyzed daily solar potential.
- **Togo:** Focused on distribution analysis and potential for consistent solar yield.

Summary statistics and visuals (histograms, time-series plots, boxplots) were generated.

---

 Cross-Country Comparison

A comparative analysis was conducted to understand how solar potential varies across the three countries. Key steps:

- Combined cleaned datasets.
- Generated side-by-side visualizations (e.g., boxplots).
- Performed ANOVA tests to evaluate statistical differences.
- Found GHI differences to be statistically significant (p < 0.05).

---

Dashboard (Streamlit)

An interactive dashboard was developed to visualize solar parameters across countries.

### Features:
- Dropdown selection for country and solar metric (GHI, DNI, DHI)
- Boxplots and statistical summaries
- Built with Streamlit and modularized for clarity

### Run the Dashboard:
```bash
streamlit run dashboard/app/main.py
