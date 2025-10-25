# 📧 Spam Mail Detection using Logistic Regression

This project uses **Logistic Regression** to classify emails as **Spam** or **Ham (Not Spam)** based on their textual content.  
The model is trained on a labeled dataset (`mail_data.csv`) containing messages categorized as either *spam* or *ham*.  
It uses **TF-IDF (Term Frequency–Inverse Document Frequency)** feature extraction for textual analysis.

---

## 📘 Project Overview

This is a **Natural Language Processing (NLP)** based **binary classification** project.  
By analyzing the words within an email, the model determines whether an incoming message is spam or not.  
The goal is to create a lightweight, interpretable, and efficient email spam filter using **Logistic Regression**.

---

## 🗂️ Dataset Information

**Dataset Name:** Mail Data  
**Format:** CSV file (`mail_data.csv`)  
**Columns:**
- **Category** → Label of the email (*ham* or *spam*)  
- **Message** → The text content of the email  

**Label Conversion:**
- `0` → Spam Mail  
- `1` → Ham Mail (Not Spam)

---

## 🧠 Technologies Used

- Python 3.x  
- NumPy  
- Pandas  
- Scikit-learn  

---

## ⚙️ Project Workflow

1. **Load the Dataset** using Pandas  
2. **Handle Missing Values** with `fillna('')`  
3. **Encode Categories** (spam → 0, ham → 1)  
4. **Split the Data** into 80% training and 20% testing  
5. **Transform Text** into numerical vectors using **TfidfVectorizer**  
6. **Train the Model** using **Logistic Regression**  
7. **Evaluate** model performance using accuracy metrics  
8. **Predict** for new custom email inputs  

---

## 📊 Example Output

Accuracy of training data : 0.97
Accuracy of testing data : 0.96

**Input Email Example:**

"Free entry in 2 a wkly comp to win FA Cup final tkts 21st May 2005. Text FA to 87121..."

**Output:**

Spam Mail

---

## 🧪 Predicting Custom Input

You can edit this variable inside the code:

input_mail = ["Your email text message here"]

The model will output either:

Spam Mail

or

The mail is Ham Mail / Not a Spam Mail

---

## 👨‍💻 Author

Developed by **Saurabh**  
Feel free to connect or contribute to this project!  

⭐ If you found this project helpful, don’t forget to **star** the repository!
