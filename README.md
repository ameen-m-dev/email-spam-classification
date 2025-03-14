# **Email Spam Classification using Machine Learning**

**Author:** Ameen Mohammad  

This project implements a **full machine learning pipeline** for spam classification.

---
### **Viewing Pre-Generated Results**
The notebook has been pre-executed, so you can explore the findings without running the code.

🔗 **[Open in Google Colab](https://colab.research.google.com/drive/1y-k7DWK4WNj2LEmyBQxx6MNBQ_Nf0vpC)** 

### **Running the Notebook (Optional)**
For those interested in running the full pipeline:
1. Open the notebook in Google Colab using the link above.  
2. Navigate to **Runtime** in the top menu and select **Run all** (or press `CTRL + F9` / `Cmd + F9` on Mac).  
3. If prompted with a security notice about execution permissions, click **"Run Anyway."**  
4. The notebook will process the dataset and generate results step by step.

## **Dataset Overview**

The dataset used in this project is a collection of **5,574 email messages**, labeled as **'spam'** or **'notspam'**. Below is a summary of the dataset:

- **Total Emails:** 5,574
- **Spam Emails:** 747 (13.4%)
- **Not Spam Emails:** 4,827 (86.6%)
- **Average Email Length:** 80 characters
- **Number of Duplicate Entries:** 406

*Note: Missing values in the 'text' column have been handled by replacing them with an empty string.*

---

## **Key Findings**

After processing the data and training multiple models, the following results were obtained:

| Model                  | Feature Extraction | Accuracy | Spam Recall | Spam F1-score |
|------------------------|--------------------|----------|-------------|---------------|
| Logistic Regression    | TF-IDF             | 95.87%   | 74%         | 85%           |
| Support Vector Machine | TF-IDF             | 97.76%   | 86%         | 92%           |
| Random Forest          | TF-IDF             | 97.49%   | 86%         | 91%           |
| Logistic Regression    | BoW                | 98.21%   | 89%         | 94%           |

**Conclusion:**

- **Best Overall Accuracy:** Logistic Regression with BoW features achieved the highest accuracy at 98.21%.
- **Best Spam Detection:** Support Vector Machine with TF-IDF features achieved the highest spam recall at 86%.

*Note: TF-IDF (Term Frequency-Inverse Document Frequency) and BoW (Bag of Words) are techniques used to convert text data into numerical features.*

---

## **Future Improvements**

To further enhance the spam classification model, the following approaches can be considered:

1. **Hybrid Feature Extraction:** Combining TF-IDF and BoW features to capture more nuances in the text data.
2. **Advanced Modeling Techniques:** Implementing deep learning models such as LSTMs or Transformers (e.g., BERT) to improve performance.
3. **Hyperparameter Tuning:** Fine-tuning the hyperparameters of the models to achieve better accuracy and recall.

---

Explore the notebook to analyze the results or modify the code to experiment with different techniques.

