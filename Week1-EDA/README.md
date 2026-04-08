# Week 1 - 🤖 Intro to Machine Learning & Cleaning, Exploratory & Visualizing Data

During this first week we took a look at the initial steps of working with data, the different machine learning models we have available to us and the importance of cleaning, exploring and visualizing our data.

## 🏆 The Challenge

The challenge had us taking a look at a dataset of bank data about it's customers and various information the bank had about them.

We explored the data. By looking at the different columns, the types of data we had and the different values in each column. We made distinctions between categorical and numerical data and did some light transformations and cleaning.

We then visualized the data using different types of plots and charts to get a better understanding of the relationships between the different features and the target variable.

Finally we applied a K-Nearest Neighbors (KNN) model to the data to make predictions about whether a customer would subscribe or not.

## 🧠 Insights

<img width="400" height="155" alt="image" src="https://github.com/user-attachments/assets/bda5d3db-86ba-46b8-be24-75b6bb6521a0" />

Looking at the classification results, we can draw several conclusions:

- The dataset is highly imbalanced: 80% no, 20% yes

- The yes category has a poor accuracy rate

- The no category has a very good accuracy rate

- Having an accuracy of 89% is misleading since some data points are classified better than others

- For a real business, we would be failing our predictions for our subscribed users
