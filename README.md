# 📊 EDA Case Studies

A collection of **real-world exploratory data analysis (EDA)** projects where I analyze diverse datasets to uncover **patterns, trends, and actionable insights** using **Python, Pandas, Matplotlib, and Seaborn**.

Each notebook is structured to reflect a complete **data exploration workflow** — from data loading to insight generation.

---

## 🧠 Goals
- Strengthen my data exploration & visualization skills  
- Build an EDA portfolio showcasing practical analysis of real datasets  
- Develop storytelling and insight communication ability  

---

## 🛠️ Tech Stack
- **Language:** Python (NumPy, Pandas)
- **Visualization:** Matplotlib, Seaborn
- **Environment:** Jupyter Notebook
- **Other Tools:** Kaggle Datasets, GitHub

---

## �️ Environment setup
Follow these PowerShell steps from the repository root (`eda-case-studies/`) to create a virtual environment and install the project dependencies listed in `requirements.txt`.

1) Create & activate a virtual environment (PowerShell):

```powershell
# Create a venv in a hidden .venv folder
python -m venv .venv

# Activate the venv in PowerShell
.venv\Scripts\Activate.ps1
```

If Activation is blocked, run:

```powershell
Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass
```

2) Upgrade pip and install dependencies:

```powershell
python -m pip install --upgrade pip setuptools wheel
pip install -r requirements.txt
```

3) (Optional) Register the venv as a Jupyter kernel so you can select it inside notebooks:

```powershell
pip install ipykernel
python -m ipykernel install --user --name eda-case-studies --display-name "EDA Case Studies (.venv)"
```

4) Add the venv to `.gitignore` to avoid committing it:

```
# Virtual environment
.venv/
```

Troubleshooting notes:
- If pip prints messages about "Ignored the following versions..." it usually means some package releases were skipped because they require a different Python version — this is informational. The fatal error in earlier installs was caused by a typo `plotlys`; the correct package name is `plotly`.
- If you see build errors on Windows for scientific packages, consider using a matching Python version (3.10/3.11) or use conda/mamba to install binary packages.

---

## �📂 Repository Structure

```
eda-case-studies/
│── 📄 README.md                  # Main overview of all projects
│── 📄 requirements.txt           # Common dependencies
│
│── 📁 airlines-flights-eda/
│   │── 📄 README.md              # Project-specific summary
│   │── 📄 airlines_eda.ipynb     # Jupyter Notebook
│   │── 📁 data/                  # dataset or link
│   │── 📁 visuals/               # charts/images
│
│── 📁 data-science-salaries-eda/
│   │── 📄 README.md
│   │── 📄 salaries_eda.ipynb
│   │── 📁 data/
│   │── 📁 visuals/
│
│── 📁 youtube-music-hits-eda/
│   │── 📄 README.md
│   │── 📄 youtube_eda.ipynb
│   │── 📁 data/
│   │── 📁 visuals/
```

---

## 📘 Case Studies

| Dataset | Source | Key Focus |
|----------|---------|-----------|
| ✈️ Airline Flights Data | [Kaggle](https://www.kaggle.com/datasets/rohitgrewal/airlines-flights-data) | Delays, cancellations, flight performance |
| 💼 Data Science Salaries 2023 | [Kaggle](https://www.kaggle.com/datasets/arnabchaki/data-science-salaries-2023) | Salary by region, experience, role |
| 🎵 YouTube Music Hits 2025 | [Kaggle](https://www.kaggle.com/datasets/ayeshaimran123/top-youtube-music-hits-2025) | Popularity trends, artist insights |

---

## 📈 Typical EDA Workflow
Each notebook follows a consistent structure:
1. **Import libraries**
2. **Load & inspect data**
3. **Clean missing and duplicate values**
4. **Univariate analysis**
5. **Bivariate & multivariate analysis**
6. **Feature engineering (if needed)**
7. **Key insights & visual storytelling**
8. **Conclusion & recommendations**

---

## 🌟 Highlights
- Hands-on with real-world, diverse datasets  
- Well-documented notebooks with clear reasoning  
- Visualizations that tell meaningful stories  

---

## 🤝 Connect with Me
I'm actively learning and sharing my journey in data exploration and analytics.  
Feel free to connect, collaborate, or share feedback!

**📧 Email:** nikumbhamit05@gmail.com 
**🔗 LinkedIn:** PLACEHOLDER
