# Data-Profiler
Understand any dataset in seconds.
https://all-formats-probe.lovable.app/
<img width="1902" height="913" alt="image" src="https://github.com/user-attachments/assets/cb1bd4ff-d30f-4861-af9c-0ab845314ca9" />

# What each report covers:
## Overview and data quality: row and column counts, missing values, duplicate rows, and alerts for problems like empty columns, skewed values or high missingness.
## Univariate: a histogram, box plot and summary statistics for each column, plus outlier counts, most frequent values and timelines for dates.
## Bivariate: pick any two columns.
Two number columns get a scatter plot with a trend line and two correlation scores.
Two category columns get a cross-tab with a test of whether they're related.
A category and a number get averages per group with a test of whether the groups differ.
There's also a grid of scatter plots for the main number columns.
## Assumptions: two normality tests for each number column, a Q–Q plot, and a check for relationships that are consistent but not straight-line.
## Multivariate (PCA): charts showing how much of the variation a few combined dimensions capture, a 2D map of the data, and how much each column contributes.
## Feature selection: which columns look most useful for modelling, which to consider dropping and why, and suggested clean-up steps (filling gaps, fixing skew, handling outliers, encoding categories).
## Documents (PDF, Word, text): word and sentence counts, a readability score, top keywords and phrases, plus any tables found inside Word files.
## Multiple files: a side-by-side comparison of all tables, with shared column names flagged as possible ways to link them.
## Export: you can download the report as a Markdown file.

# Limitations:
## Scanned PDFs: no text comes out, because there's no text recognition.
## Old .doc files: these need to be saved as .docx first.
## Spatial analysis: is not included.
## Charts: they're built into the app; it doesn't use the Python or R tools required for the analysis.
