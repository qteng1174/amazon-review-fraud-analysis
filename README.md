# Investigating the Impact of AI on Fraudulent Amazon Reviews

## Project Overview
This project analyzes large-scale Amazon review data to understand how fraudulent review behavior has evolved, particularly with the rise of AI-generated content.

The goal is to evaluate whether traditional similarity-based fraud detection methods remain effective in identifying suspicious reviews.

---

## Dataset
- ~52 million Amazon reviews
- Time range: 1996–2023
- Source: Amazon Reviews (Parquet format)

---

## Methodology
- Data processing using **PySpark on Google Cloud Dataproc**
- Similarity detection using **MinHash LSH**
- Analysis across:
  - time trends
  - product categories
  - reviewer behavior
  - text duplication patterns

---

## Key Findings

- Review volume increased significantly after 2020  
- Electronics category shows strong suspicious activity patterns  
- Some users exhibit abnormal high-volume reviewing behavior  
- Review titles are more duplicated than full text  
- Similarity detection dropped from **6.4% → 3.0% after 2022**, suggesting AI-generated paraphrasing  

---

## Conclusion
Fraudulent review behavior has shifted from direct duplication to AI-assisted paraphrasing, making traditional similarity-based detection less effective.

Future systems should incorporate semantic analysis instead of relying solely on syntactic similarity.

---

## Project Structure

The repository is organized as follows:

```text
amazon-review-fraud-analysis/
│
├── Final_Project.ipynb              # Main analysis notebook
├── amazon_review_fraud_slides.pptx # Project presentation
└── README.md

---

## Tools & Technologies
- Python  
- PySpark  
- Spark SQL  
- Google Cloud Dataproc  
- MinHash LSH  

---

## Future Work
- Apply semantic similarity models (embeddings)  
- Improve fraud detection robustness  
- Expand to other review platforms  

---

## Author
Yunelle Teng  
Applied Data Science @ University of Chicago
