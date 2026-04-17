<div align="center">

# 🏥 Medical Data Visualizer

### An Interactive Web Application for Medical Examination Data Analysis

[![Live Demo](https://img.shields.io/badge/🚀%20Live%20Demo-Click%20Here-brightgreen?style=for-the-badge)](https://medical-data-visualizer-repo-flmfq7xia75glwl2aorg5z.streamlit.app/)
[![Python](https://img.shields.io/badge/Python-3.7+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)](https://streamlit.io)
[![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org)

---

> **B.Tech CSE Minor Project — 6th Semester**
> Government College of Engineering, Keonjhar

</div>

---

## 🌐 Live Application

> **Try it now — no installation required!**
>
> 🔗 **[https://medical-data-visualizer-repo-flmfq7xia75glwl2aorg5z.streamlit.app/](https://medical-data-visualizer-repo-flmfq7xia75glwl2aorg5z.streamlit.app/)**

---

## 📋 Project Overview

**Medical Data Visualizer** is a web-based data analysis tool that uncovers patterns and correlations between lifestyle choices, body measurements, blood markers, and cardiovascular disease using real patient medical examination records.

Built with **Python** and **Streamlit**, it provides an interactive, browser-based interface requiring zero setup — just open and explore.

> Data analysis logic inspired by the [freeCodeCamp Data Analysis with Python](https://www.freecodecamp.org/learn/data-analysis-with-python/) curriculum, extended with a fully interactive Streamlit frontend.

---

## ✨ Key Features

| Feature | Description |
|---|---|
| 📊 **Categorical Plot** | Visualizes distribution of health indicators split by cardiovascular disease status |
| 🔥 **Correlation Heatmap** | Displays Pearson correlation coefficients between all numeric medical features |
| 🌐 **Interactive Web UI** | Browser-based Streamlit interface — no scripts to run manually |
| 🧹 **Data Cleaning Pipeline** | BMI classification, binary normalization, and outlier filtering |
| ✅ **Unit Tested** | Validated using Python's `unittest` framework |

---

## 📊 Visualizations

### Categorical Plot
Compares counts of **healthy (0)** vs. **unhealthy (1)** values for key health indicators — `cholesterol`, `gluc`, `smoke`, `alco`, `active`, and `overweight` — grouped by cardiovascular disease status (`cardio`).

### Correlation Heatmap
Displays **Pearson correlation coefficients** between all numeric features after filtering outliers in diastolic pressure, height, weight, and BMI — revealing which medical indicators are most strongly related to one another.

---

## 👥 Team

| # | Name | Role & Contributions |
|---|---|---|
| 1 | **Smruti Somyashree Parida** | Project setup, repository structure, `requirements.txt`, virtual environment configuration |
| 2 | **Sunayana Bal** | Data loading & preprocessing, BMI calculation, overweight column logic, outlier filtering |
| 3 | **Shrabani Parida** | Data normalization (cholesterol & glucose), `draw_cat_plot()` implementation |
| 4 | **Sulekha Deo** | `draw_heat_map()` implementation, correlation matrix logic, chart rendering |
| 5 | **Tanushree Pradhan** | Streamlit web interface (`app.py`), UI integration, testing, debugging & documentation |

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| **Python 3** | Core programming language |
| **Streamlit** | Interactive web interface |
| **Pandas** | Data loading, manipulation & cleaning |
| **Matplotlib** | Figure rendering & saving plots |
| **Seaborn** | Statistical data visualization |
| **NumPy** | Numerical operations |
| **unittest** | Automated testing framework |

---

## 🗂️ Project Structure

```
medical-data-visualizer/
│
├── app.py                       # Streamlit web app — main entry point
├── medical_data_visualizer.py   # Core logic: data processing & visualization
├── medical_examination.csv      # Dataset: patient medical examination records
├── main.py                      # Script to run visualizer & tests locally
├── test_module.py               # Unit tests for validating chart outputs
├── requirements.txt             # Python dependencies
└── README.md                    # Project documentation
```

---

## ⚙️ Local Setup

### Prerequisites
- **Python 3.7+** installed on your system

### Steps

```bash
# 1. Clone the repository
git clone https://github.com/your-username/medical-data-visualizer.git
cd medical-data-visualizer

# 2. Create and activate a virtual environment
python -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Launch the Streamlit app
streamlit run app.py
```

The app will open in your browser at **`http://localhost:8501`**

> **Optional:** Run without the web interface to generate `catplot.png` and `heatmap.png` directly:
> ```bash
> python main.py
> ```

---

## 🔗 References

- [freeCodeCamp — Data Analysis with Python](https://www.freecodecamp.org/learn/data-analysis-with-python/)
- [Streamlit Documentation](https://docs.streamlit.io/)
- [Seaborn Documentation](https://seaborn.pydata.org/)
- [Pandas Documentation](https://pandas.pydata.org/)

---

## 📄 License

This project is submitted for **academic purposes** as part of the B.Tech CSE Minor Project, 6th Semester.
Dataset sourced from the freeCodeCamp Data Analysis with Python curriculum.

---

<div align="center">

Made with ❤️ by Team Medical Data Visualizer · GCE Keonjhar · 2025

</div>
