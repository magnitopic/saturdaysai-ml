# Week 1 - 🤖 Intro to Machine Learning & Cleaning, Exploratory & Visualizing Data 

During this first week we took a look at the initial steps of working with data, the different machine learning models we have available to us and the importance of cleaning, exploring and visualizing our data.

## 🏆 The Challenge 

The challenge had us taking a look at a dataset of bank data about it's customers and various information the bank had about them.

We explored the data. By looking at the different columns, the types of data we had and the different values in each column. We made distinctions between categorical and numerical data and did some light transformations and cleaning.

We then visualized the data using different types of plots and charts to get a better understanding of the relationships between the different features and the target variable.

Finally we applied a K-Nearest Neighbors (KNN) model to the data to make predictions about whether a customer would subscribe or not.

## 📊 Visualizations

_The amount of users who have a deposit and those who don't_

<img width="589" height="432" alt="image" src="https://github.com/user-attachments/assets/2827dbdc-4ee2-4755-9027-d3971b72a950" />

---

_User distribution by ages_

<img width="580" height="432" alt="image" src="https://github.com/user-attachments/assets/0014e467-2980-48b3-ad7d-db0e5fb065b8" />

---

_Barplot of the categorical variables with the target variable_

<img width="1989" height="1173" alt="image" src="https://github.com/user-attachments/assets/a933436b-3ed6-4d14-984b-8bd232030bb3" />

---

_Pairplot to show distribution and relations of the numerical variables_

<Figure size 1823.88x1750 with 56 Axes><img width="1821" height="1790" alt="image" src="https://github.com/user-attachments/assets/593a49cd-f86a-479e-901e-3faca4777eae" />

---

_Boxplot of account balance by education level_

<img width="876" height="594" alt="image" src="https://github.com/user-attachments/assets/86af09e3-5d5d-4316-b13d-3db704310124" />

---

_Violinplot of age and type of job_

<img width="1389" height="590" alt="image" src="https://github.com/user-attachments/assets/d33fc288-6f71-468b-87b4-4deb262e2f73" />

---

_Heat map of all variables_

<img width="1859" height="1590" alt="image" src="https://github.com/user-attachments/assets/c9de15f4-66cb-443b-8486-df5307b8379b" />

---

_k-NN performace with training. Training and test_

<img width="1189" height="590" alt="image" src="https://github.com/user-attachments/assets/71bdb011-eade-4437-a25d-037ff971da9b" />

---

_Confusion matrix_

<img width="549" height="470" alt="image" src="https://github.com/user-attachments/assets/cfbaf3e8-c52e-40f3-a391-d3e11909b10b" />

---

_ROC Curve_

<img width="989" height="790" alt="image" src="https://github.com/user-attachments/assets/7d328324-b345-4618-88c5-24e4ec6588b2" />

## 🧠 Insights

<img width="400" height="155" alt="image" src="https://github.com/user-attachments/assets/bda5d3db-86ba-46b8-be24-75b6bb6521a0" />

Looking at the classification results, we can draw several conclusions:

-  The dataset is highly imbalanced: 80% no, 20% yes

-  The yes category has a poor accuracy rate

-  The no category has a very good accuracy rate

-  Having an accuracy of 89% is misleading since some data points are classified better than others

-  For a real business, we would be failing our predictions for our subscribed users
