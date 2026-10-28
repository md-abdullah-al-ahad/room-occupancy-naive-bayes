# Room Occupancy Classification with Naive Bayes

CSE 3207: Artificial Intelligence assignment — Understanding Bayes Theorem and Naive Bayes Classifier.

This repository implements a Naive Bayes classifier from scratch (NumPy/pandas only, no scikit-learn) to predict room occupancy (0–3 people) from environmental sensor readings.

Main result on the stratified 80/20 test split: **95.26% accuracy** and **0.8882 macro-F1** (2,027 test readings).

## Files
- Room_Occupancy_Naive_Bayes.ipynb: executed notebook with mathematical explanations, docstrings and inline comments.
- Occupancy_Estimation.csv: original dataset, beside the notebook as required.
- report/: LaTeX source, compiled report and the figure needed to compile it.
- results/: metrics, plots, predictions and saved split indices. The notebook creates this directory automatically.
- requirements.txt: Python dependencies.

## Run the notebook
Install the dependencies with `python -m pip install -r requirements.txt`, start `jupyter lab`,
open the notebook and run its cells in order. Keep the CSV beside the notebook.
No scikit-learn functions are used. The classifier, metrics and splits use NumPy/pandas.

## Compile the report
From report/, run `pdflatex Room_Occupancy_Report.tex` twice. Keep figures/ beside the source.
The report contains six pages in total: a contents page plus five pages of chapters and references.
No cover page is included. The source explicitly selects a Times-equivalent font via mathptmx,
12-point body text, and 1.5 line spacing via onehalfspacing. Black and navy remain the only
editorial colours; figures retain a broader palette. There are no table fills or running headers.

## Dataset attribution
Singh, A. & Chaudhari, S. (2018). Room Occupancy Estimation.
UCI Machine Learning Repository. https://doi.org/10.24432/C5P605
Creative Commons Attribution 4.0 International: https://creativecommons.org/licenses/by/4.0/
The dataset is included unchanged. Interpret findings within the controlled-room setting.
