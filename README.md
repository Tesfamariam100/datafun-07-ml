# **datafun-07-ml**

**Project Name: DataFun-07-ml**
Project Author: Tesfamariam
Date: 2024-02-18

## **Project Objective:**
Investigate how country population size in 2020 correlates with COVID-19 deaths reported in 2019 through data analysis and visualization.
Machine learning for predictive analytics

## Getting Started
Project Requirements include:
Build a model
Make predictions
Visualize the model
Publish your insights

### **Create Repository:**
In your browser, create a new GitHub repository (datafun-07-ml) with the default README.md. 

### **Clone Repository:**
Clone the newly created repository to your local machine Documents folder using `Git clone` command or via VS Code.
Git clone [my repository](https://github.com/Tesfamariam100/datafun-07-ml)

### **Create Virtual Environment:**
Set up a project virtual environment named .venv in the root project folder. In the VS Code terminal:

`python3 -m venv .venv`
Activate Virtual Environment: Activate the project virtual environment. 
In the VS Code terminal:
On Windows:
`.\.venv\Scripts\activate`

### **Manage Project Requirements:**
Install dependencies listed in the project specification.

`pip install pandas
pip install pyarrow
pip install scipy
pip install seaborn
pip install matplotlib
pip install scikit-lear`

Freeze your requirements to requirements.txt:

`pip freezerequirements.txt`

### **Add .gitignore:**
Add a useful .gitignore file to the root project folder to exclude files and directories not to be tracked by Git.

### **Document Process in README.md:**
Document the project purpose, virtual environment setup, and commands used for version control and running the code.

### **Version Control**
**Git Add and Commit:**

 - `git add .`
 - `git commit -m "Initial commit"`
 - `Git Push origin main` 

### Project Organization & Data Files
Access, download and add associated files and data to the project folder

### Project start:
create operations.ipynb file
### import the required Python libraries:

`import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression
from sklearn import metrics`

### Load the dataset into a DataFrame
`mortality_df = pd.read_csv('Mortality.csv')`

### Explore the Dataset:
Display the first few rows of the dataset
`mortality_df.head()`

### Data Preprocessing:
Check for missing values and handle them if necessary:

### Check for missing values
Perform any required data cleaning or transformations.
`mortality_df.isnull().sum()`

### Data Visualization:
Visualize the data to gain insights:
### Plotting the distribution of COVID deaths per 100,000 population

### Plotting the distribution of COVID deaths per 100,000 population

### Split the Data:

`X = mortality_df[['Population_2020']]
y = mortality_df['COVID_deaths_2019 per 100,000']
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)`

### Model Training:

Train a linear regression model using the training data:

### Initialize the linear regression model
`model = LinearRegression()`

### Fit the model to the training data
`model.fit(X_train, y_train)`

### Model Evaluation:
Evaluate the model using appropriate metrics:

# Predict on the test set
`y_pred = model.predict(X_test)`

# Calculate metrics

`Visualize the model's predictions against the actual values.`

### Conclusion and Next Steps:

Summarize your findings and discuss potential next steps or areas for further analysis.




################################################################################
# I extend special thanks to ChatGPT for their invaluable guidance and to the  # authors of 'Intro to Python for Computer Science and Data Science' by Paul J. # Deitel and Harvey Deitel (Pearson, 2020) for their insightful contributions.
################################################################################





