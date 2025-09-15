#  Alzheimer's Early Detection using Machine Learning

This project focuses on analyzing and predicting Alzheimer's disease using **exploratory data analysis (EDA)**, **feature engineering**, and **machine learning models**.  
It also provides an **interactive dashboard** to visualize key risk factors and support early screening strategies.

##  Authors
- **Jihene Guesmi**
- **Abir Jlassi**

---

##  Objectives
- Perform comprehensive EDA on Alzheimer’s disease dataset.
- Identify significant factors contributing to Alzheimer’s diagnosis.
- Develop and compare machine learning models for prediction.
- Select the best-performing model and evaluate performance.
- Provide actionable insights for healthcare professionals through dashboards.

---

##  Dataset
- **Source:** [Kaggle – Alzheimer’s Disease Dataset](https://www.kaggle.com/)  
- **Size:** 2,149 patient records  
- **Features:** 35 variables including demographic, clinical, lifestyle, and medical history factors.  
- **Target Variable:** `Diagnosis` (0 = No Alzheimer’s, 1 = Alzheimer’s)

### Key Features
- **Demographic:** Age, Gender, Ethnicity, Education Level  
- **Clinical:** MMSE Score, Functional Assessment, Memory Complaints  
- **Lifestyle:** Physical Activity, Diet Quality, Sleep Quality, Alcohol Consumption, Smoking  
- **Medical History:** BMI, Blood Pressure, Cholesterol, Diabetes, Depression  
- **Family History:** Presence of Alzheimer’s in family  

---

##  Exploratory Data Analysis (EDA)
- **Age:** Risk increases significantly after 65.  
- **MMSE Score:** Strong negative correlation with diagnosis.  
- **Family History:** 2.3x higher risk when positive.  
- **Lifestyle:** Higher physical activity and good sleep reduce risk.  
<img width="690" height="631" alt="image" src="https://github.com/user-attachments/assets/f2fb679b-0cfc-4973-907b-9682bebe0e33" />
<img width="1346" height="280" alt="image" src="https://github.com/user-attachments/assets/c23ab2ea-520c-4fe9-8d51-dc90f660c6ba" />
<img width="556" height="752" alt="image" src="https://github.com/user-attachments/assets/c88c7f6d-bcf4-4019-880d-9dc08f9b1173" />
<img width="450" height="291" alt="image" src="https://github.com/user-attachments/assets/db0b7955-119f-42bf-a5ed-dd46b6fccd15" />


---

##  Tools & Workflow
- **Languages & Libraries:**  
  - Python: `numpy`, `pandas`, `matplotlib`, `seaborn`  
  - Machine Learning: `scikit-learn`, `xgboost`  

- **Visualization:** Power BI (interactive dashboards)  
- **Workflow:**  
  1. Data preprocessing and cleaning  
  2. Feature engineering (risk score, health score, age groups)  
  3. Feature selection (top 10 features: MMSE, Age, Family History, etc.)  
  4. Model development & evaluation  
  5. Dashboard creation  

---

##  Machine Learning Models
Models Tested:
- Support Vector Machine (SVM)
- Random Forest Classifier
- K-Nearest Neighbors (KNN)
- XGBoost Classifier ✅ (best performer)

### Best Model: **XGBoost**
- Parameters: `learning_rate=0.1`, `max_depth=6`, `n_estimators=100`, `early_stopping=True`  
- Strengths:
  - Excellent handling of mixed data types
  - Robust against overfitting
  - Captures complex feature interactions  

### Most Predictive Features
- **MMSE Score** (gold standard for cognitive decline)  
- **Age**  
- **Functional Assessment**  
- **Memory Complaints**  
- **Physical Activity, Sleep Quality, Education Level, Depression History**  

---

##  Dashboarding
- Built with **Power BI**  
- Features:
  - Dynamic filtering (age groups, gender, smoking, etc.)
  - Comparative analysis across demographics & clinical metrics
  - Insights into risk factors and protective lifestyle choices  
<img width="1321" height="465" alt="image" src="https://github.com/user-attachments/assets/554b57e2-0e83-4e90-9301-850cce143b3e" />
<img width="611" height="374" alt="image" src="https://github.com/user-attachments/assets/62dfc8d0-23e6-40ac-be52-59842e983760" />
<img width="685" height="374" alt="image" src="https://github.com/user-attachments/assets/fa528e9f-618f-4805-9dbf-fa432e9dcc26" />
<img width="713" height="427" alt="image" src="https://github.com/user-attachments/assets/a92f2cd3-8c1c-4d7b-acfe-620cf80daac3" />

### Example Insights:
- Education level may delay dementia onset.  
- Behavioral symptoms (depression, aggression) align with higher diagnosis rates.  
- Preventive lifestyle factors (diet, exercise, sleep) show protective effects.  

---

##  Conclusion
This project demonstrates that combining **data analytics** and **machine learning**:
- Helps uncover Alzheimer’s patterns  
- Supports risk prediction  
- Assists healthcare professionals in early diagnosis and patient care  

---

## 📜 License
This project is licensed under the MIT License.
