# **Sentiment Analyzer (Text + Excel/CSV Input)**

A simple Gradio-based web app that performs **sentiment analysis** on:

* Multiple text lines (one per line), or
* An uploaded **Excel/CSV file** (user selects the column name)

The app uses **DistilBERT (SST-2)** for classification and generates:

* Per-line sentiment labels
* A sentiment **pie chart**

---

## 🚀 **Features**

* Accepts **manual text** or **file upload**
* User can **enter the column name**
* Supports **Excel (.xlsx/.xls)** and **CSV**
* Shows:

  * Individual predictions
  * Pie chart of sentiment distribution
* Fast inference using Hugging Face `pipeline`

---

### **`requirements.txt`**

```
torch
transformers
gradio
matplotlib
pandas
```

---

## 🧠 **Model Used**

**distilbert-base-uncased-finetuned-sst-2-english**
A lightweight, fast, and accurate sentiment classifier from Hugging Face.

---

## 📝 **How to Use**

### **Option 1: Paste text**

* Enter multiple reviews/comments
* One line = one prediction

### **Option 2: Upload Excel/CSV**

* File must contain a text column
* Enter the **column name** in the input box

---

## 📊 **Output**

* **Left:** Each line with its predicted sentiment
* **Right:** A matplotlib-based **Pie Chart** for sentiment distribution

