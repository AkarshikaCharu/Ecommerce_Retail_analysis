# Ecommerce_Retail_analysis
This notebook performs sentiment analysis on e-commerce product reviews using **TextBlob** for polarity scoring and NLTK for text preprocessing.
E-commerce Customer Sentiment Analysis
This project analyzes a dataset of 5,000 customer reviews to determine the emotional tone (Positive, Negative, or Neutral) of each entry. 
It includes text preprocessing steps such as stopword removal and keyword extraction to prepare data for further analysis or machine learning.

Project Overview
The notebook follows a structured data science workflow:
Data Loading: Imports a CSV containing product reviews and original sentiment labels.
Sentiment Scoring: Utilizes `TextBlob` to calculate a `polarity_score` for every review.
Classification: Categorizes scores into 'Positive' (> 0), 'Negative' (< 0), and 'Neutral' (0).
Text Cleaning: Uses `NLTK` to remove common English stopwords and filter for alphabetic keywords.
Export: Saves the enriched dataset as `sentiment_analysis_final.csv`.

Dataset Structure
The original dataset (`ecommerce-product-reviews.csv`) contains:
review: The raw text of the customer's feedback.
label: The original sentiment classification.

The processed output adds:
polarity_score: A numerical value between -1.0 and 1.0.
sentiment analysis: The calculated category based on the polarity score.
keywords: Cleaned text containing only meaningful, lowercase alphabetic words.

Key Findings
Upon analysis, the sentiment distribution of the 5,000 reviews was found to be:
| Sentiment | Count |
| Positive | 3,501 |
| Negative | 1,088 |
| Neutral| 411 |

Requirements
To run this notebook, you will need the following Python libraries:

* `pandas`
* `numpy`
* `matplotlib`
* `textblob`
* `nltk`

 How to Use
1. Clone the repository and ensure the `ecommerce-product-reviews.csv` file is in the same directory (or update the file path in the first cell).
2. Install dependencies using `pip install pandas textblob nltk`.
3. Run the cells sequentially to process the text and generate the sentiment report.
4. Download the results: The final cell will automatically trigger a download of the processed CSV if running in Google Colab.
