# Public Opinion Analysis Using NLP

*An NLP-based public opinion analysis project that processes social media posts from X to perform sentiment classification, topic modeling, and interactive visualization through a responsive web interface.*

## 📌 The Problem

Public discussions on social media generate large volumes of text that are difficult to analyze manually. For policy-related discussions, identifying sentiment patterns and recurring topics can help researchers understand the main themes expressed in the collected dataset.

This project focuses on analyzing public opinion surrounding **Government Regulation (PP) Number 47 of 2024** using text data collected from the social media platform X.

## 💡 The Solution

Developed an NLP pipeline that combines **sentiment analysis**, **topic modeling**, and **interactive web visualization**.

The project collects posts and replies from X using **Tweet Harvest**, followed by text preprocessing, translation, manual sentiment labeling, Naive Bayes classification, and Latent Dirichlet Allocation (LDA) topic modeling.

The analysis results are integrated into a responsive website that provides sentiment charts, wordcloud visualization, LDA exploration, research methodology, reports, and downloadable research data.

The main workflow consists of:

1. Collecting posts and replies from X using selected keywords.
2. Cleaning and preprocessing the text data.
3. Translating the processed dataset from Indonesian to English.
4. Manually labeling text into positive, neutral, and negative sentiment categories.
5. Training and evaluating a Naive Bayes sentiment classifier.
6. Applying LDA to identify dominant discussion topics.
7. Generating sentiment, wordcloud, and LDA visualizations.
8. Presenting the results through a responsive web interface.

## 🚀 The Impact / Results

* **879 raw records** were collected from X using three main keywords during the 2024 observation period.
* After preprocessing, the dataset was reduced to **778 cleaned records** ready for analysis.
* The sentiment distribution in the detailed results consisted of **326 positive (41.90%)**, **426 neutral (54.76%)**, and **26 negative (3.34%)** records.
* The Naive Bayes model achieved a reported accuracy of **73.65%** in the detailed results and conclusion. The abstract reports **72.62%**.
* LDA identified **three major themes** related to debt relief, the role of the president, and public support or appreciation toward the policy.
* The final analysis was presented through a responsive website with interactive **Bar Chart**, **Wordcloud**, and **LDA Model** visualizations, alongside methodology, report, and data download pages.

## 📂 Repository Structure

The repository contains the research datasets, machine learning and topic-model outputs, Jupyter notebooks, and the responsive analysis website.

```text
nlp-public-opinion-analysis/
├── README.md
│
├── datasets/
│   ├── Data Sentimen/
│   ├── hasilCrawling/
│   ├── hasilLDA/
│   ├── hasilPreprocessing/
│   ├── hasilTerjemahan/
│   ├── hasil_visualisasi/
│   ├── manualCrawling/
│   └── normalisasiLDA/
│
├── models/
│
├── notebooks/
│   ├── crawling_data.ipynb
│   └── sentiment_analysis_naive_bayes.ipynb
│
└── website/
    ├── index.html
    ├── bar-chart.html
    ├── wordcloud.html
    ├── lda-model.html
    ├── methodology.html
    ├── report.html
    ├── download.html
    │
    ├── css/
    │   └── style.css
    │
    └── asset/
        ├── Bar Chart.png
        ├── Data Sentimen.csv
        ├── df_dominant_topic.csv
        ├── df_imp_wcount.csv
        ├── Latar Belakang Penelitian.pdf
        ├── PP Nomor 47 Tahun 2024.pdf
        └── Wordcloud Topic.png
```

## 🛠️ Tech Stack

* **Python**
* **Google Colab**
* **Tweet Harvest**
* **Playwright**
* **googletrans**
* **TextBlob**
* **Naive Bayes Classifier**
* **Gensim**
* **Latent Dirichlet Allocation (LDA)**
* **LDAvis**
* **HTML / CSS**
* **CSV / Excel**

## 📸 Project Gallery

### Sentiment Distribution

<p align="center">
  <img src="website/asset/Bar Chart.png" alt="Sentiment Distribution Bar Chart" width="700">
</p>

### Wordcloud

<p align="center">
  <img src="website/asset/Wordcloud Topic.png" alt="Wordcloud Visualization" width="700">
</p>

### Interactive Analysis Website

The project includes a responsive web interface for exploring the analysis results:

* [Home / Dashboard](website/index.html)
* [Bar Chart](website/bar-chart.html)
* [Wordcloud](website/wordcloud.html)
* [LDA Model](website/lda-model.html)
* [Methodology](website/methodology.html)
* [Research Report](website/report.html)
* [Download Data](website/download.html)

### LDA Analysis Output

* [LDAvis Interactive Output](datasets/hasilLDA/ldavis_prepared_3.html)
* [Sentiment Chart Output](datasets/hasil_visualisasi/bar_chart_sentimen.html)
* [Wordcloud Output](datasets/hasil_visualisasi/wordcloud_sentimen.html)
