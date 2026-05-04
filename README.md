# Sentiment Analysis using DistilBERT (Fine-Tuning)

## 📌 Project Overview
This project builds a sentiment analysis model to classify customer product reviews as **Positive** or **Negative** using a pre-trained transformer model (DistilBERT).

---

## ❗ Problem Statement
A consumer electronics company needs an automated system to analyze customer reviews. Manual analysis is slow and inefficient, so this project uses NLP to classify sentiment automatically.

---

## 🎯 Objective
- Build a sentiment classification system  
- Use a pre-trained NLP model (DistilBERT)  
- Fine-tune on a small dataset (800 samples)  
- Evaluate model performance  

---

## 🛠️ Technologies Used
- Python  
- Google Colab  
- Hugging Face Transformers  
- PyTorch  
- Scikit-learn  

---

## 📊 Dataset
- **Source:** Amazon Product Reviews (amazon_polarity)  
- **Samples Used:** 800  

### Label Mapping:
- `0` → Negative  
- `1` → Positive  

---

## ⚙️ Methodology

### 1. Data Collection
Loaded dataset using Hugging Face and selected 800 samples.

### 2. Data Preprocessing
- Extracted review text  
- Used original labels  
- Split into training (80%) and testing (20%)

### 3. Tokenization
Converted text into tokens using DistilBERT tokenizer with padding and truncation.

### 4. Dataset Preparation
Created a custom PyTorch dataset class to convert data into tensors.

### 5. Model Selection
Used **DistilBERT**, a lightweight transformer model.

### 6. Fine-Tuning
- Trained for 2 epochs  
- Batch size: 8  
- Used Hugging Face Trainer API  

### 7. Evaluation
Measured performance using:
- Accuracy  
- Precision  
- Recall  
- F1-score  

### 8. Inference
Tested model on custom inputs:
   "This phone is amazing" → Positive
  "Worst product ever" → Negative

---

## 🏗️ System Architecture
User Input (Text)
↓
Preprocessing
↓
Tokenization (DistilBERT)
↓
DistilBERT Model (Fine-Tuned)
↓
Classification Layer
↓
Sentiment Output (Positive / Negative)


---

## 📈 Results
- Model successfully classifies sentiment  
- Achieved good accuracy with small dataset  
- Demonstrates effectiveness of transfer learning  

---

## 🧠 Key Concepts
- Natural Language Processing (NLP)  
- Transfer Learning  
- Transformers  
- Tokenization  
- Fine-Tuning  

---

## ⚠️ Challenges
- Small dataset size  
- Initial labeling issues  
- Slow training on CPU  

---

## ✅ Solutions
- Used pre-trained model  
- Corrected label mapping  
- Used Google Colab (GPU support)  

---

## 🚀 Future Improvements
- Use larger dataset  
- Add neutral sentiment class  
- Improve accuracy with tuning  
- Deploy as API  

---

## 📌 Conclusion
This project shows how a pre-trained transformer like DistilBERT can be fine-tuned on a small dataset to perform sentiment analysis effectively.

---

## 📎 Deliverables
- Google Colab Notebook  
- Working sentiment classification model  
  
