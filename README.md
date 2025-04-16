# 🩺 Diabetes Risk Assessment Tool

This is a Streamlit-based web application that predicts the risk of diabetes using health parameters such as glucose level, BMI, insulin, age, and more. It is powered by a logistic regression model trained on the Pima Indians Diabetes Dataset.

> ⚠️ **Note**: This tool is for informational purposes only and does not substitute professional medical advice.

---

## 🚀 Features

- 🔍 **Diabetes Risk Prediction** based on 8 medical attributes
- 📈 **Visual Probability Meter** (Progress bar)
- 🟢 **Risk Level Indicator** (Low / Moderate / High)
- 🩺 **Personalized Health Recommendations**
- 📊 **Feature Importance Visualization** using odds ratio
- 📚 **Educational Insight** into each contributing factor

---

## 💡 Tech Stack

- **Frontend/UI**: [Streamlit](https://streamlit.io/)
- **Model**: Logistic Regression (`sklearn.linear_model`)
- **Data Preprocessing**:
  - `pandas`, `numpy`, `SimpleImputer`, `StandardScaler`
- **Data**: Pima Indians Diabetes Dataset (`diabetes.csv`)

---

## 🧠 How It Works

1. **Data Preprocessing**:
   - Missing or zero values in columns like Glucose, BMI, etc., are imputed using the mean.
   - Features are standardized for model training.

2. **Model Training**:
   - Logistic Regression model is trained to classify diabetic vs. non-diabetic.
   - Caching is used to prevent retraining on every run.

3. **User Input via Sidebar**:
   - Input fields for:
     - Pregnancies
     - Glucose
     - Blood Pressure
     - Skin Thickness
     - Insulin
     - BMI
     - Diabetes Pedigree Function
     - Age

4. **Risk Assessment**:
   - The model outputs a **probability of diabetes**.
   - Results include a visual meter, risk category, and tailored health tips.

5. **Explanation & Education**:
   - Bar chart shows the **impact of each feature**.
   - Written explanations help users understand the role of each factor.

---

## 📷 Screenshot

<img width="563" alt="image" src="https://github.com/user-attachments/assets/b95c6111-14b8-4236-890c-66cb32dca1a8" />


---

## 🏁 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/your-username/your-repo.git
cd your-repo

2. Install dependencies
bash
Copy
Edit
pip install -r requirements.txt
3. Add the dataset
Place your diabetes.csv file in the root directory. You can find it here.

4. Run the app
bash
Copy
Edit
streamlit run app.py
