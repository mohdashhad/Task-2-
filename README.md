# Task-2-
# 🕸️ Web Scraping & Keyword Analysis – Dubai Travel Websites

This project scrapes content from top Dubai travel websites, performs keyword extraction (including bigrams and trigrams), and analyzes keywords based on competition and tail length. The final output is a structured Excel report.

---

## 🔗 Target Websites

1. [TripAdvisor - Dubai](https://www.tripadvisor.in/Tourism-g295424-Dubai_Emirate_of_Dubai-Vacations.html)
2. [The Sophisticated Life - Dubai Guide](https://thesophisticatedlife.com/blog/dubai-travel-guide-first-time-visitors/)
3. [Expedia - Dubai](https://www.expedia.co.in/Dubai.dx6053839)

---

## ⚙️ Features

- Scrapes:
  - Page title
  - Meta description
  - H1–H3 tags
  - Full body text (excluding scripts/styles)
- Performs:
  - Text preprocessing (cleaning, stopword removal)
  - Tokenization
  - N-gram generation (unigrams, bigrams, trigrams)
- Analyzes:
  - Keyword frequency (used as a proxy for competition)
  - Keyword tail length (`short-tail`, `mid-tail`, `long-tail`)
  - Ranks keywords from **high-to-low competition**
  - Sorts from **long-to-short tail**
- Exports results to Excel

---

## 📁 Output

- `keyword_analysis_report.xlsx`  
  Contains:
  - `keyword`
  - `frequency`
  - `tail_type` (short-tail/mid-tail/long-tail)
  - `competition` (1 = highest competition)

---

## 🧪 Requirements

Install required libraries:
```bash
pip install requests beautifulsoup4 pandas nltk
