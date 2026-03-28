# 🏥 Medical Data Visualizer

> **B.Tech CSE Minor Project — 6th Semester**
> **Government College of Engineering, Keonjhar**
> Guided By ~

> An interactive web application for visualizing and analyzing medical examination data using Python and Streamlit.

---

## 📋 Project Overview

This project is a **web-based medical data visualization tool** developed as a minor project for the 6th Semester B.Tech CSE program. It analyzes patient medical examination records to uncover patterns and correlations between lifestyle choices, body measurements, blood markers, and cardiovascular disease.

The application is built using **Python** for data analysis and **Streamlit** for an interactive web interface, allowing users to explore two key visualizations directly in the browser — without any setup complexity.

The data analysis logic was inspired by the [freeCodeCamp Data Analysis with Python](https://www.freecodecamp.org/learn/data-analysis-with-python/) curriculum and extended with a fully interactive Streamlit frontend developed by the team.

---

## 👥 Team Members & Contributions

This project was collaboratively developed by a team of 5 students as part of the **6th Semester B.Tech CSE Minor Project**.

| # | Name | Contributions |
|---|---|---|
| 1 | **Smruti Somyashree Parida** | Project setup, repository structure, `requirements.txt`, virtual environment configuration |
| 2 | **Sunayana Bal** | Data loading & preprocessing, BMI calculation, overweight column logic, outlier filtering |
| 3 | **Shrabani Parida** | Data normalization (cholesterol & glucose), `draw_cat_plot()` implementation |
| 4 | **Sulekha Deo** | `draw_heat_map()` implementation, correlation matrix logic, chart rendering |
| 5 | **Tanushree Pradhan** | Streamlit web interface (`app.py`), UI integration, testing, debugging & documentation |

---

## ✨ Features

- 📊 **Categorical Plot** — Visualizes the distribution of health indicators (cholesterol, glucose, smoking, alcohol, activity, overweight) split by cardiovascular disease status
- 🔥 **Correlation Heatmap** — Displays Pearson correlation coefficients between all numeric medical features after outlier removal
- 🌐 **Streamlit Web Interface** — Interactive browser-based UI to view both charts without running scripts manually
- 🧹 **Data Cleaning Pipeline** — BMI-based overweight classification, binary normalization of cholesterol & glucose, and outlier filtering
- ✅ **Unit Tested** — Validated using Python's `unittest` framework

---

## 🗂️ Project Structure

```
medical-data-visualizer/
│
├── app.py                       # Streamlit web app — main entry point
├── medical_data_visualizer.py   # Core logic: data processing & visualization functions
├── medical_examination.csv      # Dataset: patient medical examination records
├── main.py                      # Script to run visualizer & tests locally
├── test_module.py               # Unit tests for validating chart outputs
├── requirements.txt             # Python dependencies
└── README.md                    # Project documentation
```

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| Python 3 | Core programming language |
| Streamlit | Interactive web interface |
| Pandas | Data loading, manipulation & cleaning |
| Matplotlib | Figure rendering & saving plots |
| Seaborn | Statistical data visualization |
| NumPy | Numerical operations |
| unittest | Automated testing |

---

## ⚙️ Setup & Installation

### Prerequisites
Make sure you have **Python 3.7+** installed on your system.

### Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/medical-data-visualizer.git
   cd medical-data-visualizer
   ```

2. **Create a virtual environment** *(recommended)*
   ```bash
   python -m venv venv
   source venv/bin/activate        # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the Streamlit web app**
   ```bash
   streamlit run app.py
   ```
   This will open the application in your browser at `http://localhost:8501`

5. *(Optional)* **Run without the web interface**
   ```bash
   python main.py
   ```
   This generates `catplot.png` and `heatmap.png` directly in the project folder.

---

## 📊 Output Visualizations

### Categorical Plot
Compares counts of healthy (0) vs. unhealthy (1) values for features — `cholesterol`, `gluc`, `smoke`, `alco`, `active`, and `overweight` — split by cardiovascular disease status (`cardio`).

### Correlation Heatmap
Shows Pearson correlation coefficients between all numeric features after filtering outliers in diastolic pressure, height, weight, and BMI. Helps identify which medical indicators are most strongly related.

---

## 🔗 References

- [freeCodeCamp - Data Analysis with Python](https://www.freecodecamp.org/learn/data-analysis-with-python/)
- [Streamlit Documentation](https://docs.streamlit.io/)
- [Seaborn Documentation](https://seaborn.pydata.org/)
- [Pandas Documentation](https://pandas.pydata.org/)

---

## 📄 License

This project is submitted for academic purposes as part of the B.Tech CSE Minor Project (6th Semester). Dataset sourced from the freeCodeCamp Data Analysis with Python curriculum.
