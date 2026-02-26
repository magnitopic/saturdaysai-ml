# Week 2 - 📊 Basic ML Models & Evaluation Metrics

During this second week we deepened our understanding of machine learning fundamentals by working with the k-Nearest Neighbors (k-NN) algorithm and exploring various evaluation metrics to assess model performance. We learned how different metrics like accuracy, precision, recall, F1-score, and ROC curves help us understand our model's strengths and weaknesses.

## 🏆 The Challenge

The challenge focused on the famous **Pima Indians Diabetes Database** from the National Institute of Diabetes and Digestive and Kidney Diseases. This dataset contains medical information about female patients of at least 21 years of age with Pima Indian heritage.

We analyzed various medical features to predict diabetes:

- **Pregnancies** - Number of previous pregnancies
- **Glucose** - Plasma glucose concentration (2-hour oral glucose tolerance test)
- **BloodPressure** - Diastolic blood pressure (mm Hg)
- **SkinThickness** - Triceps skin fold thickness (mm)
- **Insulin** - 2-hour serum insulin (U/ml)
- **BMI** - Body mass index (weight in kg/(height in m)²)
- **DiabetesPedigreeFunction** - Diabetes pedigree function (scores diabetes probability based on family history)
- **Age** - Age in years
- **Outcome** - Target variable (0 = No diabetes, 1 = Has diabetes)

We performed exploratory data analysis, handled missing values, normalized the data, and built a k-NN classifier to predict diabetes presence. The key focus was on understanding and interpreting various evaluation metrics to properly assess our model's performance.

## 📊 Visualizations

_Distribution of patients with and without diabetes_

<img width="571" height="432" alt="image" src="https://github.com/user-attachments/assets/47ad73a6-b3c3-42d4-93a1-5b2c23259dd3" />

---

_Age distribution across the dataset_

<img width="1229" height="778" alt="image" src="https://github.com/user-attachments/assets/3d296118-2a07-4e22-8fd2-c958bea5af18" />

---

_Pairplot of all features_

<img width="2060" height="1967" alt="image" src="https://github.com/user-attachments/assets/5873abf0-b91e-4d44-a28f-da4b437f627f" />

---

_Blood pressure, age comparison for diabetes_

<img width="571" height="432" alt="image" src="https://github.com/user-attachments/assets/fce46886-25e2-4b03-9dd0-ae019095d30a" />

---

_Glucose distribution for diabetes_

<img width="571" height="455" alt="image" src="https://github.com/user-attachments/assets/02fe0a26-3647-4d9a-9b8a-81f07e1108c4" />

---

_Correlation heatmap of all features_

<img width="1732" height="1588" alt="image" src="https://github.com/user-attachments/assets/24ce9184-c578-40f3-a0f4-e69a58e5310d" />

---

_k-NN error rate vs number of neighbors (k)_

<img width="855" height="547" alt="image" src="https://github.com/user-attachments/assets/e0d9f150-7ada-4f6a-9966-b802f546a07b" />

---

_k-NN accuracy vs number of neighbors (k)_

<img width="855" height="547" alt="image" src="https://github.com/user-attachments/assets/e500e885-567a-4a06-aa88-7538f35bbc9c" />

---

_Confusion matrix for the final model_

<img width="649" height="547" alt="image" src="https://github.com/user-attachments/assets/35bced84-e5a3-4319-af75-1a90334c9cb7" />

---

_ROC Curve with AUC score_

<img width="536" height="547" alt="image" src="https://github.com/user-attachments/assets/afb4569b-77a1-4760-96ba-3bc59242f1cb" />

## 🧠 Insights

### Model Performance

After testing different values of k (number of neighbors), we found the optimal k-value that balanced bias and variance:

- **AUC Score: 0.78** - The model has a 78% probability of correctly distinguishing between diabetic and non-diabetic patients
- The model shows acceptable/good performance for a baseline classifier
- Training and test scores indicate good generalization without significant overfitting

### Key Findings

**Evaluation Metrics Understanding:**

- **Accuracy** alone can be misleading, especially with imbalanced datasets
- **Precision vs Recall** trade-off is important for medical applications where false negatives can be costly
- **F1-Score** provides a balanced measure when both precision and recall matter
- **ROC Curve** helps visualize the model's ability to separate classes across different thresholds

**ROC Curve Analysis:**

- The curve rises rapidly at the beginning, indicating the model identifies many true positives without many false positives initially
- Being significantly above the diagonal reference line (random classifier) confirms effective learning
- The closer the curve is to the top-left corner, the better the model's performance

**Medical Context:**

- For diabetes prediction, the balance between sensitivity (detecting actual diabetes cases) and specificity (avoiding false alarms) is crucial
- The k-NN algorithm with normalized features performs reasonably well for this classification task
- Feature engineering and proper data normalization are essential for distance-based algorithms like k-NN
