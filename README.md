# 📰 Fake News Detector

A project that uses NLP, Machine Learning, and Deep Learning to figure out if a news article is fake or real.

## 👥 Team
- Nishil Patel (SID: 202201166)  
- Jainil Patel (SID: 202201030)  

## 🎯 What We Tried to Do
We wanted to solve a simple but important problem: is a news article trustworthy?  
To do that, we built a bunch of models using classical ML and GloVe-based deep learning.  
Then, we combined the best of them into an ensemble model to get more reliable predictions.

## 🔧 Tech Stack & Libraries
- Text Processing: NLTK, re, string  
- ML Models: sklearn (Naive Bayes, Logistic Regression)  
- Deep Learning: TensorFlow, Keras  
- Embeddings: GloVe (glove.6B.300d.txt)  
- Interface: Gradio  
- Deployment: Hugging Face Spaces

## 📂 Files in This Project
- app.py → Main Gradio app  
- model.pkl → ML model (TF-IDF + Naive Bayes / Logistic Regression)  
- model.h5 → Deep Learning model (GloVe + DNN)  
- tokenizer.pkl → Tokenizer used with GloVe  
- requirements.txt → Dependencies  
- glove.6B.300d.txt → Pre-trained word embeddings  
- README.md → This file  

## 🧠 How It Works
1. Input news text  
2. We clean and process it  
3. Run it through ML and DL models  
4. Combine predictions using a weighted ensemble  
5. Show the result (Fake or Real) with confidence score

## 📊 Model Scores

| Model               | Accuracy | F1 (Fake) | F1 (Real) |
|--------------------|----------|-----------|-----------|
| Naive Bayes        | 85%      | 0.87      | 0.83      |
| Logistic Regression| 93%      | 0.94      | 0.92      |
| GloVe + DNN        | 90.55%   | –         | –         |

## 🚀 Deployment
This project is live on Hugging Face Spaces using Gradio.  
- Try it here 👉 https://jainilp30-fake-news-detector.hf.space  
- Dataset Link 👉 [Dataset](https://www.kaggle.com/datasets/stevenpeutz/misinformation-fake-news-text-dataset-79k)

### Libraries and Tools Used:
- 🧠 [GloVe Embeddings by Stanford NLP](https://nlp.stanford.edu/projects/glove/)  
- 🌐 [Gradio Interface Library](https://www.gradio.app/)  
- 📚 [scikit-learn](https://scikit-learn.org/) for model implementation  
- 🛠 [NLTK](https://www.nltk.org/) for basic NLP preprocessing  

## 📜 License
MIT License

## ⚠️ Disclaimer
This project is built purely for educational and experimental purposes to explore basic Natural Language Processing (NLP) and ML/DL techniques. It is not suitable for real-world fact-checking or decision-making. The models used are simple, non-contextual, and cannot understand language nuances or factual correctness. Misusing this tool for serious analysis may lead to incorrect or harmful conclusions. Please do not trust or rely on the outputs of this demo. It is meant for learning only.

## Demo
![image](https://github.com/user-attachments/assets/d2c38988-0299-458c-b63c-c9ada7c8eb7a)  
![image](https://github.com/user-attachments/assets/23a4fba6-47a6-459a-94a2-7d8425c93387)
