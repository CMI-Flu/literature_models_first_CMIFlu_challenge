# Comparative-analysis-CMI-Flu
## Comparative analysis of vaccine prediction models using datasets from the CMI-Flu project

This repository includes all of the code used to implement and compare models predictive of vaccine responses.

Briefly summarized, a literature review was performed to identify previously presented methods for predicting vaccine responses. First, 40 papers were selected from the literature search using keyword searches and relevant references in other papers. From the 40 papers 13 studies were confirmed to present relevant prediction methods based on the selection two criteria, 1) the predictive framework should be utilizing baseline i.e. pre-vaccination measurements, which either established clear biological differences between vaccine responders and non-responder, explicitly predicted antibody titers, or classified subjects according to their vaccine-induced antibody response, and 2) the data used to establish the predictive frameworks should be based on data, which is also present in the CMI-Flu project. For several of the 13 relevant studies, multiple prediction methods were presented. In total, 24 prediction methods were implemented from 10 of the relevant 13 studies. The prediction methods that obtained significant results for both performance metrics in the CMI-Flu training resource dataset were also evaluated in the CMI-Flu 2025 (UGA cohort) dataset.


The repository contains a folder containing an R Markdown file of the workflow for evaluating the prediction models in each of the 10 studies included in the project.

The first step is to download the data used in this project. This can be accomplished by running the scripts `download_from_webpage_links.sh` to download the data files and `Standardize_data.ipynb` to preprocess the data files.

- After the data has been downloaded and processed, the Rmarkdown files for each of the studies can be run. These files contain the workflows for evaluating all of the prediction methods included in this project.

- Finally, the comparative analysis can be run to compare the results from all of the prediction methods.
