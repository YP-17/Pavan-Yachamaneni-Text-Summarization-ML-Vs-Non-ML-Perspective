# Pavan-Yachamaneni-Text-Summarization-ML-Vs-Non-ML-Perspective
This repo is the course project for the CMSE 890 course Advanced Machine Learning. 

# Project Title: Text Summarization - An ML vs Non-ML Perspective
## Dataset
cnn_dailymail dataset from Kaggle

## Project Details
This project presents a comparative study of ML algorithms - Seq2Seq autoencoder and pre-trained T5 model, and a non-ML algorithm - TextRank, for text summarization.

## Project File Description
* `Data_prep_cnn_dailymail.ipynb`: This file contains a custom function to clean the data, and applies techniques such as removing stop words, handling text contractions, lemmatizing, regex operations, tokenization, and padding.
* `EDA_cnn_dailymail.ipynb`: This file contains detailed EDA techniques such as dataset distribution, word frequency analysis, stop word removal, and n-grams.
* `T5.ipynb`: This file takes the cleaned text from `Data_prep_cnn_dailymail.ipynb` and uses the T5 pre-trained model provided by Hugging Face.
* `TextRank.ipynb`: This file implements the TextRank algorithm.
* `Seq2Seq.ipynb`: This file implements the Seq2Seq autoencoder model and presents the results of all three models.
* `Report.pdf`: A detailed report with more information.

## Results and Conclusion
After evaluating the three models using the ROUGE metric, we obtained the following scores:

| Model    | ROUGE-1 | ROUGE-2 | ROUGE-L |
| -------- | ------- | ------- | ------- |
| TextRank | 0.254   | 0.093   | 0.218   |
| Seq2Seq  | 0.308   | 0.119   | 0.264   |
| T5       | 0.392   | 0.186   | 0.337   |


Based on these scores, we can see that the T5 model outperforms the other two models across all ROUGE metrics, while the Seq2Seq model has the lowest ROUGE scores. This suggests that the T5 model may be the most effective at generating high-quality summaries. However, it's important to note that these results may vary depending on the specific dataset and summarization task being evaluated.



