# -Ass17.1
## Exploratory Data Analysis

![image](https://github.com/Soha1950/-Ass17.1/assets/160794678/25532e2a-c77a-427d-bf5f-949f58222247)

Based on the graph, we can see that the average age of customers, whether they have subscribed to a fixed deposit or not, is approximately between 38 and 40 years. The significant overlap in the boxplots for both groups suggests that age is not a strong predictor of whether a customer will subscribe to a fixed deposit.

![image](https://github.com/Soha1950/-Ass17.1/assets/160794678/8e9dc641-d19b-49d7-9b68-81b21f7343d4)

This type of graph is very useful for comparing the distribution of a variable, such as age, among different groups, such as target groups. However, FacetGrid is most effective for visualizing age distributions in the 20-30 year range and for ages 60 and older.
![image](https://github.com/Soha1950/-Ass17.1/assets/160794678/c8c5f4b0-bd3d-4617-b997-8aca216ec093)
![image](https://github.com/Soha1950/-Ass17.1/assets/160794678/6586d1f2-910f-4c7d-93ff-fcbc0b83901d)

95% of people having age are less than equal to 58.0
96% of people having age are less than equal to 59.0
97% of people having age are less than equal to 59.0
98% of people having age are less than equal to 62.0
99% of people having age are less than equal to 71.0
100% of people having age are less than equal to 98.0
IQR 15.0
![image](https://github.com/Soha1950/-Ass17.1/assets/160794678/401ad602-01e2-4162-8ad2-cfdec9c60408)

![image](https://github.com/Soha1950/-Ass17.1/assets/160794678/c735791a-c7f4-4eb4-b2a1-1d384acc4818)

The graph above shows that the duration of the last contact with the customer is a useful predictor of the target variable. In fact, the longer the contact duration, the more likely the response is positive. This is consistent with the data overview, which indicates that this field strongly affects the target variable and should only be used for benchmarking purposes.

![image](https://github.com/Soha1950/-Ass17.1/assets/160794678/d3128e05-68b7-4c6b-8e9d-5297b7bcdaef)
![image](https://github.com/Soha1950/-Ass17.1/assets/160794678/6782eaf5-74a7-4c67-b1c0-b45971f0c229)
![image](https://github.com/Soha1950/-Ass17.1/assets/160794678/e5e3be38-58ac-4e63-8325-1ac0a357f516)
The graph above indicates that customers with admin jobs have the highest rates of both term deposit subscriptions and non-subscriptions. This is simply because there are more clients in admin roles than in any other profession.


![image](https://github.com/Soha1950/-Ass17.1/assets/160794678/b4e345ac-e704-4e28-911f-1d80521476fb)
![image](https://github.com/Soha1950/-Ass17.1/assets/160794678/67b6eb39-7871-40fa-a5de-323a85319637)
The majority of the customers are married.

![image](https://github.com/Soha1950/-Ass17.1/assets/160794678/3ac3d54d-dc43-4751-840f-c1a238e44dfd)

![image](https://github.com/Soha1950/-Ass17.1/assets/160794678/655f83cf-a599-4acf-a0f0-6eb0707a70b9)

![image](https://github.com/Soha1950/-Ass17.1/assets/160794678/c28df055-49b5-449f-92ce-6f1fd0312430)

![image](https://github.com/Soha1950/-Ass17.1/assets/160794678/f130de2d-5d85-4168-941a-76b3d2e19db4)

![image](https://github.com/Soha1950/-Ass17.1/assets/160794678/cb65502d-c600-4116-9db2-bd23be6910b5)
The chart above illustrates the bank's call rate and customer response rate for each month, with the trend lines moving in different directions. This can be interpreted in two ways: either the bank increases its calls when demand for deposits declines, or the timing of the calls is suboptimal. The highest call rates occurred in May and August, while the highest subscription rates were in March and September.

![image](https://github.com/Soha1950/-Ass17.1/assets/160794678/80711c98-aae0-45a0-be62-852e648bbe0a)

It's apparent that certain numerical features display notable correlations. For instance, "nr.employed" and "euribor3m" exhibit a correlation coefficient of 0.95, while "euribor3m" and "emp.var.rate" show a correlation of 0.97. These correlations stand out as exceptionally high when compared to others observed in the heatmap.

![image](https://github.com/Soha1950/-Ass17.1/assets/160794678/3d662958-d7bd-4e50-a432-166dcbb96efc)

The feature duration has the highest importance by a significant margin.
Other features like euribor3m, age, nr.employed, and job also have noticeable importance.
Features like default, contact, loan, and previous have the least importance.
This plot is crucial for understanding which features contribute the most to the model's predictions, potentially guiding feature selection and further analysis. 

![image](https://github.com/Soha1950/-Ass17.1/assets/160794678/ad1d2783-21f8-4f4c-90e2-6673708a152b)


# Left Plot (PCA for Discretised Dataset):

X-axis: Represents the principal components.
Y-axis: Represents the variance explained by each principal component.
The first few principal components explain a significant portion of the variance, with the first component explaining the most.

# Right Plot (PCA for Continuous Dataset):

X-axis: Represents the principal components.
Y-axis: Represents the variance explained by each principal component.
Similarly, the first few principal components explain a significant portion of the variance, with the first component explaining the most.


![image](https://github.com/Soha1950/-Ass17.1/assets/160794678/875f3d35-e8ed-4c97-b96f-58155202020a)

# Left Plot: 2D PCA Projection
### Title: "First two PCA directions"
Axes:
X-axis: Represents the first principal component (PC1).
Y-axis: Represents the second principal component (PC2).
### Data Points:
Data points are colored based on the target variable y, with two classes: 0 (navy) and 1 (darkorange).
Each point represents an observation from the dataset, projected onto the first two principal components.
Legend: Indicates the classes (0 and 1) with their respective colors.
Purpose: This plot shows how the dataset can be represented in a lower-dimensional space (2D) while retaining as much variance as possible. It helps visualize the separation or overlap between different classes.
# Right Plot: 3D PCA Projection
### Title: "First three PCA directions"
Axes:
X-axis: Represents the first principal component (PC1).
Y-axis: Represents the second principal component (PC2).
Z-axis: Represents the third principal component (PC3).
### Data Points:
Similar to the 2D plot, data points are colored based on the target variable y, with two classes: 0 (navy) and 1 (darkorange).
Each point represents an observation from the dataset, projected onto the first three principal components.
Legend: Indicates the classes (0 and 1) with their respective colors.
Purpose: This plot extends the visualization to three dimensions, providing a more comprehensive view of the data structure and the relationships between classes. The 3D perspective helps identify any additional patterns or separations that may not be evident in the 2D plot.

	
# Classification Algorithms¶

The algorithms compared are Decision Tree (Tree), K-Nearest Neighbors (KNN), Logistic Regression, and Support Vector Machine (SVM). Each algorithm is represented by a different colored bar, and the accuracy is measured on the training data.

![image](https://github.com/Soha1950/-Ass17.1/assets/160794678/b769a569-6d4b-42d5-83e5-3a7666bfc995)


Each bar represents the accuracy of a specific algorithm.
Tree: Accuracy is approximately 0.889.
KNN: Accuracy is approximately 0.902.
LogisticRegression: Accuracy is approximately 0.910.
SVM: Accuracy is approximately 0.912.
The color of each bar corresponds to a different algorithm as indicated by the legend on the right side of the chart.
Summary of the Accuracy Scores:
SVM has the highest training data accuracy at approximately 0.912.
LogisticRegression follows closely with a training accuracy of approximately 0.910.
KNN has a training accuracy of approximately 0.902.
Tree (Decision Tree) has the lowest training accuracy among the compared algorithms at approximately 0.889.
Interpretation:
High Training Accuracy: All algorithms exhibit high training accuracy, with SVM and Logistic Regression performing slightly better than KNN and Tree.


