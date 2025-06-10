# 📱 Ethiopian Banks App Review Scraper & Analyzer

This project collects, preprocesses, and analyzes Google Play Store reviews for mobile banking apps of three major Ethiopian banks:

- **Commercial Bank of Ethiopia (CBE)**
- **Bank of Abyssinia (BOA)**
- **Dashen Bank**

The goal is to simulate real-world consulting scenarios in product, marketing, and engineering using app review insights.

---

## 🔍 Project Scenarios

### Scenario 1: Retaining Users
- Identify common user complaints such as slow transfers.
- Analyze if these issues are widespread.

### Scenario 2: Enhancing Features
- Extract common feature requests (e.g., fingerprint login, fast loading).
- Recommend feature improvements per bank.

### Scenario 3: Managing Complaints
- Cluster complaints for integration into AI-based support.
- Help guide faster support resolution.

---

## 🧪 Methodology

### 1. **Data Collection**
- Used the `google-play-scraper` Python package to fetch the latest 400 reviews for each bank.
- Retrieved the following metadata: review content, star rating, review date, and app identifier.
- Stored all reviews in a combined DataFrame with the bank name as a new column.

### 2. **Preprocessing**
- Removed duplicate entries.
- Checked and handled missing values.
- Normalized dates to `YYYY-MM-DD` format.
- Selected relevant columns: `review`, `rating`, `date`, `bank`, and `source` (optional).

### 3. **Analysis**
- Calculated review volume per bank to assess user engagement.
- Measured percentage of missing data to evaluate data quality.
- Performed exploratory text analysis to extract complaint themes and feature requests.
- Categorized reviews based on scenario relevance (performance issues, feature requests, support complaints).

---

## 🚀 Features

- Web scraping using `google-play-scraper`
- Collection of 400+ reviews per app
- Preprocessing and cleaning (deduplication, null handling, date normalization)
- Summary statistics (review count, missing data %)
- Scenario-based textual analysis

---

## 🛠️ Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/Amenzz/week-2.git
    cd week-2
