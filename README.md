# WeRateDogs Twitter Archive Analysis

This project wrangles and analyzes data from the **WeRateDogs** Twitter account. It combines tweet metadata, image predictions, and engagement metrics to explore how users interact with dog‑related content on Twitter.

## Dataset
The following files form the basis of the analysis:

- `twitter-archive-enhanced.csv` – Original tweet data supplied by WeRateDogs.
- `image-predictions.tsv` – Machine learning predictions of the dog breed appearing in each tweet's image.
- `Twitter_archive_master.csv` – Cleaned master dataset produced after combining and tidying all sources.

Additional notebooks and scripts in this repository demonstrate the wrangling process and exploratory analysis.

## Data Wrangling Summary
The data required extensive cleaning to address missing values, inconsistent data types, and erroneous entries. Important steps included:

1. Converting timestamps and other fields to appropriate types.
2. Removing or correcting records with inaccurate information.
3. Creating new features such as dog age and engagement totals.
4. Merging the image predictions and additional tweet metrics into a single master table.

Details of these steps can be found in `wrangle_act.ipynb` and the accompanying `wrangle_report.pdf`.

## Summary of Findings
Analysis of the cleaned dataset revealed several insights:

- Tweets that include **videos** tend to receive more likes and retweets than those containing only images.
- Machine learning predictions of dog breeds were often inconsistent, limiting breed‑specific conclusions.
- Dog names in the dataset do not necessarily correspond to breed information and are sometimes missing or incorrect.

These observations highlight the challenges of working with user‑generated content and automated image classification. Full exploration and visualizations are available in `act_report.ipynb` and `act_report.pdf`.

## Repository Contents
- `wrangle_act.ipynb` – Notebook used to clean and merge the raw datasets.
- `wrangle_report.ipynb`/`wrangle_report.pdf` – Documentation of the wrangling approach.
- `act_report.ipynb`/`act_report.pdf` – Exploratory analysis and final report of key findings.
- `twitter-api.py` – Script used to gather additional data via the Twitter API.

---
Created by **Abdulmjeed Adahasi** as part of the Udacity Data Analyst Nanodegree.
