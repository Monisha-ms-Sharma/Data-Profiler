# Data Profiler

Understand any dataset in seconds.  
[https://dataprofiler.app](https://dataprofiler.app)

<img width="1920" height="973" alt="Data Profiler" src="https://github.com/user-attachments/assets/0d608973-7bd5-498d-a026-8b3f9b6f0a5b" />

# Exploratory Data Analysis (EDA) Studio

An automated, browser-based Exploratory Data Analysis application that turns raw data files into structured, statistical, and visual reports in seconds.

Upload single or multiple files in virtually any common format. The app cleans, profiles, checks statistical assumptions, detects anomalies, and generates both visual dashboards and narrative AI summaries—all completely inside your browser.

---

## What this app is about

Exploratory Data Analysis (EDA) is usually the most time-consuming phase of any data project. Analysts often write hundreds of lines of boilerplate code in Python or R just to inspect distributions, find correlations, verify assumptions, and spot data quality issues.

Data Profiler automates that entire initial discovery phase. Drop in your data files, and it immediately computes statistical summaries, runs hypothesis tests, maps coordinates, highlights data risks, and explains what the numbers mean in both novice-friendly plain English and data-science technical views—without writing a single line of code.

---

## What it can do

- **Reads 11+ formats**: CSV, TSV, Excel (`.xlsx`, `.xls`), Parquet, Feather/Arrow, JSON, JSON Lines, SQL dumps, XML, text documents, Word (`.docx`), PDF, and `.zip` archives.
- **Strict full-dataset evaluation**: Evaluates 100% of your records with zero silent downsampling. If a file exceeds browser memory, the app provides explicit splitting instructions to preserve every row.
- **Profiles tables and documents**: Handles structured relational tables as well as unstructured text documents.
- **Evaluates data relationships**: Computes centered Pearson and Spearman correlations, cross-tabulations, normality tests, and PCA dimensionality reduction.
- **Includes spatial analysis**: Detects latitude and longitude coordinates to produce point density maps, hotspot clusters, and spatial autocorrelation metrics (Moran's I, Nearest Neighbor Index).
- **Interactive 3-level visual drill-downs**: Click any chart or data mark across views to open a pop-up drill down with breadcrumb history, breakdown selectors, and matching raw records.
- **Domain & governance recognition**: Automatically recognizes column patterns across 41 industry and governance domains with built-in healthcare privacy notices.
- **DIY exploratory tools**: Global Focus filters, custom arithmetic column formulas evaluated over complete records, and saved-view libraries.
- **Executive & white-label exports**: Download publisher-branded executive dossiers (PDF, Markdown, Excel/CSV) or generate white-label customized reports with your own logo and company branding.
- **Two-way BI Hub interoperability**: Direct handoff and session compatibility with Business Intelligence Hub.

---

## What to expect from this app

1. **Private by default**: Raw files never leave your machine. Parsing, arithmetic, charting, and statistical tests execute entirely client-side in your browser.
2. **Instant diagnostics**: Within seconds of loading, get clear warnings about missing fields, skewed columns, duplicates, and data leakage risks.
3. **Actionable, data-grounded guidance**: Recommendations and insights are strictly derived from your loaded records, avoiding generic assumptions.
4. **Plain English & Technical Views**: Toggle between clear business explanations and rigorous statistical language.
5. **No software installation**: Runs straight from any modern browser—no Python, R, Jupyter notebooks, or database servers required.

---

## What each report covers

### Overview and data quality
- Row and column counts, dataset memory size, and file format metadata.
- Missing values count and percentage across every column with clear conversion diagnostics.
- Duplicate row detection and constant/zero-variance column alerts.
- Inferred subject domain recognition and data dictionary summaries.

### Univariate analysis
- Histograms, box plots, and complete descriptive statistics (Mean, Median, Sample Standard Deviation, IQR, Min, Max, Skewness, Kurtosis).
- Outlier detection via IQR boundaries with affected-record inspection.
- Cardinality percentages and top value distributions for categorical columns.
- Timelines, date spans, and frequency trends for temporal columns.

### Bivariate analysis
- **Two numeric columns**: Scatter plot with automatic trend lines, centered Pearson correlation, and Spearman rank scores.
- **Two categorical columns**: Contingency cross-tabulation table with Chi-Square test of independence.
- **Category vs. numeric**: Group distributions and ANOVA / t-test comparisons showing group separation.
- **Correlation matrix**: High-performance correlation heatmap and pairwise scatter plot matrices.

### Assumptions & reliability
- Skewness/kurtosis ratios, normality diagnostics, and Kolmogorov-Smirnov distance metrics.
- Interactive Q–Q (Quantile-Quantile) plots comparing empirical data against theoretical Gaussian distributions.
- Monotonicity and variance consistency checks.

### Multivariate (PCA)
- Principal Component Analysis over standardized numeric columns.
- Scree plot highlighting explained variance ratios across components.
- 2D biplot projection mapping individual records along principal axes.
- Component loadings matrix detailing original variable contributions.

### Spatial analysis
- Automatic coordinate detection (Latitude/Longitude) or manual column assignment.
- Geographic centroid and bounding-box spatial coverage.
- Interactive point distribution maps and 2D spatial density hotspot grids.
- Spatial autocorrelation tests: **Moran’s I** and **Nearest Neighbor Index (NNI)**.

### Feature selection & modeling readiness
- Identification of informative columns for downstream machine learning.
- Dropping recommendations (e.g., constant fields, unique ID leakage, collinear pairs with \(|r| > 0.85\)).
- Data cleaning playbooks: imputation guidance, skew transformations, and categorical encoding advice.

### Four Types of Analytics & AI Analyst
- **Descriptive**: What happened in this dataset?
- **Diagnostic**: Why did it happen (drivers, correlations, anomalies)?
- **Predictive**: What patterns or historical trends are likely to continue?
- **Prescriptive**: What concrete actions should be taken, ranked by confidence and priority?
- **AI Analyst**: Contextual question-answering with prompt suggestions and narrative summaries.

### Documents (PDF, Word, text)
- Word, sentence, and character counts.
- Readability scores (Flesch Reading Ease and Flesch-Kincaid Grade Level).
- Lexical diversity (vocabulary richness) and top n-gram phrase frequencies.
- Structural analysis including page estimates and embedded table extraction from Word documents.

### Multiple files & comparison
- Side-by-side comparison of schema structures across uploaded tables.
- Automatic detection of shared keys and join opportunities.
- One-click merging when schemas match identically.

### Exporting & sharing
- **Executive PDF**: Multi-page report containing statistical tables, charts, alerts, and analytical findings.
- **Markdown & Excel/CSV**: Clean `.md` exports for documentation tools and full-row workbooks for spreadsheet analysis.
- **Customized White-Label Reports**: Client-branded PDF/HTML exports stripped of all application branding.
- **BI Hub Sessions**: Seamless export and import for Business Intelligence Hub.

---

## 16 Built-in Sample Dataset Models

Explore full platform capabilities immediately using deterministic 1,200-row sample datasets across 16 domains:
- Finance & Banking
- Healthcare & Clinical
- E-commerce & Retail
- Cybersecurity & Threat Intel
- Space & Aviation
- Industrial Manufacturing
- Bio Sciences & Genetics
- Geospatial & Urban Planning
- Food & Tourism
- Media & Entertainment
- Corporate Governance
- Human Resources
- Business Analysis
- System Analysis & Operations
- Environment & Climate
- Mining & Extraction

---

## Technical limitations & file handling

- **Scanned PDFs**: Text cannot be extracted from image-only scanned PDFs (no optical character recognition / OCR).
- **Legacy `.doc` files**: Binary Word documents must be saved in modern `.docx` format before uploading.
- **Complete-data memory limits**: Large datasets that exceed available browser memory are not silently sampled; the app prompts you to split the file without losing records.
- **Encrypted files**: Password-protected spreadsheets or PDFs must have security removed prior to upload.
