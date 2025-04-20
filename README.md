# 🏆 Awesome Python Resources

A curated list of useful **GitHub repositories and Python libraries** with explanations and links.

---

## 🚀 Python Libraries

### 🔹 Machine Learning & AI
- [**Scikit-Learn**](https://github.com/scikit-learn/scikit-learn) - Simple and efficient tools for predictive data analysis.
- [**TensorFlow**](https://github.com/tensorflow/tensorflow) - An open-source library for deep learning models.
- [**PyTorch**](https://github.com/pytorch/pytorch) - A deep learning framework for flexible neural networks.
- [**Optuna**](https://github.com/optuna/optuna) - A hyperparameter optimization framework for machine learning.
- [**Nevergrad**](https://github.com/facebookresearch/nevergrad) - Python library for derivative-free and evolutionary optimization, useful for hyperparameter tuning and black-box optimization.
- [**PyCaret**](https://github.com/pycaret/pycaret) - A low-code machine learning library that automates data preprocessing, model selection, and hyperparameter tuning for rapid prototyping.
- [**PyTorch-Lightning**](https://github.com/Lightning-AI/lightning) - A lightweight PyTorch wrapper that automates boilerplate code and streamlines **model training**.
- [**cvxpylayers**](https://github.com/cvxgrp/cvxpylayers) - A differentiable convex optimization layer for PyTorch and TensorFlow, enabling end-to-end training with constrained optimization problems.

### 🔹 Data Science & Visualization
- [**Pandas**](https://github.com/pandas-dev/pandas) - Data manipulation and analysis tool.
- [**Matplotlib**](https://github.com/matplotlib/matplotlib) - A plotting library for Python.
- [**Seaborn**](https://github.com/mwaskom/seaborn) - Statistical data visualization built on Matplotlib.
- [**HyperTools**](https://github.com/ContextLab/hypertools) - A visualization library that helps analyze high-dimensional data.
- [**Mito**](https://github.com/mito-ds/mito) - A spreadsheet UI for Jupyter notebooks that allows interactive data manipulation and automatically generates corresponding Python code.
- [**pygwalker**](https://github.com/Kanaries/pygwalker) - A tool that combines Python and GraphWalker to enable interactive, code-free exploratory data analysis.
- [**Data Formulator**](https://github.com/microsoft/data-formulator) - Microsoft's **no-code AI-powered data analysis** tool with a **drag-and-drop UI** for visualization tasks.
- [**PivotTableJS**](https://github.com/nicolaskruchten/pivottable) - Lets you **interactively analyze data** in Jupyter Notebooks without writing any code.
- [**DrawData**](https://github.com/koaning/drawdata) - Allows you to draw **2D datasets** of any shape inside a Jupyter Notebook—great for ML algorithm understanding.
- [**Lux**](https://github.com/lux-org/lux) - A Python library that facilitates fast and easy data exploration by automatically suggesting relevant visualizations.
  ```python
  import lux
  import pandas as pd
  df = pd.read_csv("dataset.csv")
  df  # Lux automatically suggests visualizations
  ```
- [**Skimpy**](https://github.com/aeturnum/skimpy) - A lightweight tool for quickly generating summary statistics and visualizations from pandas DataFrames.
  ```python
  import skimpy
  report = skimpy.skim(df)
  report.display()  # Shows comprehensive data summary
  ```
- [**Jupiter-DataTables**](https://github.com/jupyter-datatables/jupyter-datatables) - An interactive table widget for Jupyter notebooks that enhances data exploration with filtering, searching, and visualization capabilities.
  ```python
  from jupyter_datatables import init
  init()
  display(df)  # Shows an interactive data table
  ```

### 🔹 Web Development
- [**Flask**](https://github.com/pallets/flask) - Lightweight web framework for Python.
- [**Django**](https://github.com/django/django) - High-level web framework that encourages rapid development.

### 🔹 Data Quality & Preprocessing
- [**Cleanlab**](https://github.com/cleanlab/cleanlab) - A library for identifying and correcting label errors in datasets, improving the quality of training data for ML models.
- [**Featuretools**](https://github.com/alteryx/featuretools) - An automated feature engineering library that generates meaningful features from temporal datasets.
- [**FireDucks**](https://fireducks-dev.github.io/) - Speeds up Pandas by **20x** with a simple one-line code change:
  ```python
  import fireducks.pandas as pd
  ```
- [**Black**](https://github.com/psf/black) - The **uncompromising Python code formatter** that keeps your code clean and consistent.


### 🔹 Time Series Analysis
- [**stumpy**](https://lnkd.in/eX5YJEA3) - A powerful and scalable library for computing matrix profiles, enabling time-series anomaly detection, motif discovery, and segmentation.
- [**PySINDy**](https://lnkd.in/etB7Stsd) - A library for sparse identification of dynamical systems (SINDy), enabling discovery of governing equations from time-series data.

### 🔹 Explainable AI & Interpretability
- [**Shapash**](https://github.com/MAIF/shapash) - A machine learning explainability library that simplifies the interpretation of model predictions.
- [**AIX360**](https://github.com/Trusted-AI/AIX360) - An interpretability toolkit that provides a collection of explainable AI algorithms for black-box and transparent ML models.
- [**CometML Opik**](https://github.com/comet-ml/opik) - An **open-source LLM evaluation platform** that helps test and monitor LLM applications in development and production.

### 🔹 Data Scraping
- [**MarkItDown**](https://github.com/microsoft/markitdown) - A lightweight Python utility for converting various files to Markdown for use with LLMs and related text analysis pipelines.
- [**Crawl4AI**](https://github.com/unclecode/crawl4ai) - A **web scraping tool** designed for AI applications, making data extraction easy and AI-ready.
- [**Beautiful Soup**](https://github.com/wention/BeautifulSoup4) - A library for scraping information from web pages by providing Pythonic idioms for iterating, searching, and modifying the parse tree.
  ```python
  from bs4 import BeautifulSoup
  import requests
  
  response = requests.get("https://example.com")
  soup = BeautifulSoup(response.text, "html.parser")
  titles = soup.find_all("h1")  # Extract all h1 elements
  ```

### 🔹 GUI & Web Apps
- [**Taipy**](https://github.com/Avaiga/taipy) - A low-code Python framework for building interactive data science applications, including pipelines, dashboards, and AI-driven workflows.
- [**Streamlit**](https://github.com/streamlit/streamlit) - A fast way to build and share data apps with minimal code, turning data scripts into shareable web apps in minutes.
  ```python
  import streamlit as st
  
  st.title("Simple Streamlit App")
  user_input = st.text_input("Enter some text")
  if st.button("Process"):
      st.write(f"You entered: {user_input}")
  ```
- [**PyQt**](https://github.com/PyQt5/PyQt) - Python bindings for the Qt application framework, enabling the development of rich GUI applications.
- [**Gradio**](https://github.com/gradio-app/gradio) - Creates customizable UI components for machine learning models that anyone can use right in their browser.

### 🔹 Developer Tools & Productivity
- [**Reloading**](https://github.com/julvo/reloading) - A small utility that enables automatic reloading of Python modules, making it easier to iterate on code without restarting the kernel.
- [**LazyPredict**](https://github.com/shankarpandala/lazypredict) - Enables training, testing, and evaluation of multiple ML models in just a few lines of code for both regression & classification.
- [**PandasAI**](https://github.com/gventuri/pandas-ai) - Integrates generative AI with pandas, allowing you to interact with DataFrames using natural language.

---

## 🌟 Useful GitHub Repositories

### 🔹 Python Learning Resources
- [**Awesome Python**](https://github.com/vinta/awesome-python) - A comprehensive list of Python frameworks, libraries, and resources.
- [**Real Python**](https://github.com/realpython) - Tutorials and articles for learning Python.

### 🔹 Algorithmic Trading
- [**Backtrader**](https://github.com/mementum/backtrader) - Backtesting library for trading strategies.
- [**QuantConnect**](https://github.com/QuantConnect/Lean) - Algorithmic trading engine.

---

## 💡 Contributing
Feel free to **fork** this repo, add more resources, and submit a **pull request**!
