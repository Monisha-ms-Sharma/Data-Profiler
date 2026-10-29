# Data-Profiler
Understand any dataset in seconds.
https://all-formats-probe.lovable.app/
<img width="1902" height="913" alt="image" src="https://github.com/user-attachments/assets/cb1bd4ff-d30f-4861-af9c-0ab845314ca9" />

# Exploratory Data Analysis (EDA) Studio

An automated, browser-based Exploratory Data Analysis application that turns raw data files into structured, statistical, and visual reports in seconds.

Upload single or multiple files in virtually any common format. The app cleans, profiles, checks statistical assumptions, detects anomalies, and generates both visual dashboards and narrative AI summaries—all completely inside your browser.

---

## What this app is about

Exploratory Data Analysis (EDA) is usually the most time-consuming phase of any data project. Analysts typically have to write hundreds of lines of Python or R code just to check distributions, find correlations, verify assumptions, and spot data quality problems.

This app automates that entire initial cycle. You drop in your data files, and it immediately computes statistical summaries, runs hypothesis tests, maps coordinates, highlights risks, and explains what the numbers mean—without writing a single line of code.

---

## What it can do

- **Reads 11+ formats**: CSV, TSV, Excel (`.xlsx`, `.xls`), Parquet, Feather/Arrow, JSON, JSON Lines, SQL dumps, XML, text documents, Word (`.docx`), PDF, and `.zip` archives.
- **Big data ready**: Uses streaming chunking and reservoir sampling to smoothly process files with hundreds of thousands or millions of rows (tested up to 1.5M+ rows) without freezing your browser.
- **Analyzes tables and text**: Profiles structured tabular data as well as unstructured text and documents.
- **Evaluates data relationships**: Computes correlations, bivariate comparisons, normality tests, and PCA dimensionality reduction.
- **Includes spatial analysis**: Automatically detects latitude/longitude coordinates to produce point density maps, hotspot clusters, and spatial autocorrelation scores.
- **Generates executive deliverables**: Lets you ask AI questions about your data, produces a "Four Types of Analytics" briefing, and exports everything to formatted PDF or Markdown.

---

## What to expect from this app

1. **Private by default**: Your raw files stay on your machine. Data parsing, math, charts, and statistics run entirely client-side in your browser.
2. **Instant diagnostics**: Within seconds of uploading, you get clear warnings about missing fields, skewed columns, duplicates, and data leakage risks.
3. **Actionable guidance**: Rather than just showing numbers, the app tells you *why* a column might be problematic and suggests concrete cleanup and feature-selection steps.
4. **No software installation**: Runs straight from any modern web browser—no Python, R, Jupyter notebooks, or SQL database setup required.

---

## What each report covers

### Overview and data quality
- Row and column counts, dataset memory size, and file format details.
- Missing values count and percentage across every column.
- Duplicate row detection.
- Proactive quality alerts for empty columns, highly skewed values, uniform/zero-variance fields, or excessive missingness.

### Univariate analysis
- A histogram, box plot, and full summary statistics for each column (Mean, Median, Standard Deviation, IQR, Min, Max, Skewness, Kurtosis).
- Outlier counts and ranges detected via IQR boundaries.
- Most frequent values and cardinality percentages for category columns.
- Timelines, date spans, and frequency trends for date/time columns.

### Bivariate analysis
Pick any two columns to explore how they interact:
- **Two number columns**: Scatter plot with an automatic trend line, plus both Pearson (linear) and Spearman (rank) correlation scores.
- **Two category columns**: Contingency cross-tabulation table with a Chi-Square test of independence to see whether they are significantly related.
- **A category and a number**: Group averages, distributions, and a test (t-test / ANOVA) showing whether the group averages differ meaningfully.
- **Correlation grid**: A full correlation matrix and pairwise scatter plot grid for all key numerical fields.

### Assumptions
- Two normality tests for each numerical column (skewness/kurtosis ratios and Gaussian goodness-of-fit).
- Interactive Q–Q (Quantile-Quantile) plots comparing your data against a theoretical normal bell curve.
- Checks for monotonic relationships that are consistent but not straight lines.

### Multivariate (PCA)
- Principal Component Analysis running on all standardized numeric columns.
- Scree plot showing how much of the total dataset variance the first few combined dimensions capture.
- 2D scatter projection (biplot) mapping your data points across the principal components.
- Component loadings table detailing how much each original column contributes to each component.

### Spatial analysis
- Automatic detection of latitude and longitude coordinate columns (or manual selection).
- Centroid (geographic center point) and bounding box spatial extent.
- Interactive point distribution map and 2D spatial density grid highlighting geographic hotspots.
- Spatial autocorrelation tests: **Moran’s I** (clustered vs. dispersed vs. random) and **Nearest Neighbor Index (NNI)**.

### Feature selection
- Recommendations on which columns look most useful for downstream predictive modeling.
- Clear flags on which columns to consider dropping and why (e.g., constant columns, unique identifier leaks, collinear pairs with \(|r| > 0.85\)).
- Suggested cleanup steps: strategies for imputing missing values, transformations to fix skew, outlier capping, and categorical encoding.

### Dual AI Intelligence
- **AI Insights**: Ask specific questions or provide business context; the model highlights non-obvious patterns, flags subtle risks, and recommends next analytical steps.
- **Four Types of Analytics Report**: Automatically structures your data into the four classic analytical pillars:
  - *Descriptive*: What happened in this dataset?
  - *Diagnostic*: Why did it happen (root drivers and anomalies)?
  - *Predictive*: What patterns or trends are likely to continue?
  - *Prescriptive*: What concrete actions should be taken (tagged with priority and confidence)?

### Documents (PDF, Word, text)
- Word, sentence, and character counts.
- Readability scores (Flesch Reading Ease and Flesch-Kincaid Grade Level).
- Lexical diversity (vocabulary richness) and top frequent keywords and n-gram phrases.
- Document structure breakdown, including page estimates and extraction of tables found inside Word documents.

### Multiple files
- Side-by-side comparison of all uploaded tables.
- Automatic schema comparison showing matching vs. differing column sets.
- Shared column names flagged as potential keys to join or link files together.
- One-click merging when files share the exact same schema.

### Export
- **Download PDF**: A multi-page, formatted executive dossier containing overview stats, data dictionaries, correlation tables, normality checks, alerts, and the full AI narrative.
- **Download Markdown**: A clean `.md` document ready for GitHub, Notion, or internal wikis.

---

## Limitations

- **Scanned PDFs**: Text cannot be extracted from scanned image-only PDFs because the app does not currently include optical character recognition (OCR).
- **Old `.doc` files**: Legacy Word binary files are not supported directly; they need to be saved as modern `.docx` format first.
- **Device memory limits**: Very large datasets (e.g., >500,000 rows) are automatically sampled using statistical reservoir sampling to keep your browser tab fast and prevent out-of-memory crashes.
- **Encrypted files**: Password-protected spreadsheets or encrypted PDFs must have passwords removed before uploading.
- **Offline AI**: Core statistics, charts, spatial metrics, and exports work completely offline, but AI narrative features require an internet connection.
- **Built-in charts**: Visualizations are rendered natively in the browser via Web standards; the app does not run or require external Python (`matplotlib`/`seaborn`) or R (`ggplot2`) environments.
