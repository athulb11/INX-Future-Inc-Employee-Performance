# INX-Future-Inc-Employee-Performance

## Business Case
INX Future Inc , (referred as INX ) , is one of the leading data analytics and automation solutions provider with over 15 years of global business presence. INX is consistently rated as top 20 best employers past 5 years. INX human resource policies are considered as employee friendly and widely perceived as best practices in the industry.

Recent years, the employee performance indexes are not healthy and this is becoming a growing concerns among the top management. There has been increased escalations on service delivery and client satisfaction levels came down by 8 percentage points.

CEO, Mr. Brain, knows the issues but concerned to take any actions in penalizing non-performing employees as this would affect the employee morale of all the employees in general and may further reduce the performance

## Project Goals
1. Department wise performances

After analysis, reports shows that Sales, Human Resource, Development, Research and Development and Finance departments have a performance rating of '3' which according to business standards is Satisfactory.
Data Science has employee ratings of '3' and '4', but it has some employees having a rating of '2', which according to business standard is unsatisfactory.

2. Top 3 Important Factors effecting employee performance

The most important features are EmpEnvironmentSatisfaction followed by YearsSinceLastPromotion and EmpDepartment.

3. A trained model which can predict the employee performance based on factors as inputs. This will be used to hire employees

Best performing models to predict the performance of the employees are with accuracy scores are:
Random Forest Classifier :- 97%
Gradient Boosting :- 96%
Decision Tree with best hyperparameter :- 95%

4. Recommendations to improve the employee performance based on insights from analysis.

Create a positive and supportive work environment: Employees who feel valued and appreciated are likelier to be engaged and productive.Improve environment in which the employee works by giving Flexible working hours,Refreshment area,provide more fun activities.

Promote Employees more often in order to make them feel more job oriented.

Employee may be want to switch department in order to grow but aren't able to do so, also results in declining performance.

Provide training opportunities: Support employee development with individual coaching, workshops, courses, seminars, job shadowing, mentoring, tuition reimbursement, and increasing job responsibilities.

## Analysis
Complete Domain analysis was done on each and every feature to squeeze out maximum information that would help in analyzing.

Feature was divided into categorical and Numerical in order to perform analysis.

The features tell the relation between the dependent and independent variables.

Feature importance was used to bring out the most important feature which affects in the companies growth.

#### Numerical Features
Age

DistanceFromHome

EmpHourlyRate

NumCompaniesWorked

EmpLastSalaryHikePercent

TotalWorkExperienceInYears

TrainingTimesLastYear

ExperienceYearsAtThisCompany

ExperienceYearsInCurrentRole

YearsSinceLastPromotion

YearsWithCurrManager

#### Categorical Features
EmpNumber

Gender

EducationBackground

MaritalStatus

EmpDepartment

EmpJobRole

BusinessTravelFrequency

OverTime

Attrition

#### Data
Data Background

External

The data was extracted from the link provided by IABAC.

This data is from INX future Inc, where they wanted to explore Machine learning in order to benifit their organization.

The provider had demanded certain reports that need to be speecified and executed.

Processed

This dataset went under many analysis process in order to extract insights that would be helpful for the organization.

Various Visualization Techniques as well as Pre-processing techniques were used to transform the raw dataset into a proper model building dataset.

Many trial and error have been performed in order to achieve the maximum results.

Raw

This dataset was in raw excel form.

This data set had a collection of Employee details such as (Age,Gender,job role, etc)

This Raw data set has 1200 rows and 28 columns

#### Source Code
Pandas - Pandas is a popular Python library for data analysis. It is not directly related to Machine Learning. As we know that the dataset must be prepared before training. In this case, Pandas comes handy as it was developed specifically for data extraction and preparation. It provides high-level data structures and wide variety tools for data analysis. It provides many inbuilt methods for grouping, combining and filtering data.

Numpy - NumPy is a very popular python library for large multi-dimensional array and matrix processing, with the help of a large collection of high-level mathematical functions. It is very useful for fundamental scientific computations in Machine Learning. It is particularly useful for linear algebra, Fourier transform, and random number capabilities.

Seaborn - Seaborn is another open-source Python library, one that is based on Matplotlib (which focuses on plotting and data visualization) but features Pandas’ data structures. Seaborn is often used in ML projects because it can generate plots of learning data. Of all the Python libraries, it produces the most aesthetically pleasing graphs and plots, making it an effective choice if you’ll also use it for marketing and data analysis.

Scipy - SciPy is a very popular library among Machine Learning enthusiasts as it contains different modules for optimization, linear algebra, integration and statistics. There is a difference between the SciPy library and the SciPy stack. The SciPy is one of the core packages that make up the SciPy stack. SciPy is also very useful for image manipulation.

Scikit-learn - Scikit-learn is one of the most popular ML libraries for classical ML algorithms. It is built on top of two basic Python libraries, viz., NumPy and SciPy. Scikit-learn supports most of the supervised and unsupervised learning algorithms. Scikit-learn can also be used for data-mining and data-analysis, which makes it a great tool who is starting out with ML

Matplotlib - Matplotlib is a very popular Python library for data visualization. Like Pandas, it is not directly related to Machine Learning. It particularly comes in handy when a programmer wants to visualize the patterns in the data. It is a 2D plotting library used for creating 2D graphs and plots. It provides various kinds of graphs and plots for data visualization, viz., histogram, error charts, bar chats, etc,

#### Data Visualization
Univariate - Univariate analysis is the simplest kind of data analysis in the field of statistics. This could be either descriptive or inferential in nature as is the case in any data analysis in statistics. The key thing about the univariate analysis to remember is that there is only one data involved here. While the univariate analysis may be easy to analyze and also is not complex, at times it may end up giving some misleading information especially if there are more variables involved. In this case, you need to move to the bivariate and the multivariate analysis that will be capable of analyzing the data better.

Bivariate Analysis - It is a methodical statistical technique applied to a pair of variables (features/ attributes) of data to determine the empirical relationship between them. In order words, it is meant to determine any concurrent relationship between different variables.

Multivariate Analysis - Multiple regression is the most commonly utilized multivariate technique. It examines the relationship between a single metric dependent variable and two or more metric independent variables.

Library Used: Matplotlib & Seaborn

Plots Used: Histplot, Lineplot, CountPlot, Barplot

Tip: All Observation or insights written below the plots

## CONCLUSION
There are some features are positively correlated with performance rating( Target variable) such as Emp Environment, Emp Satisfaction, Emp Last Salary Hike Percent, Emp Work Life Balance

All Basic checks have been successfully verified.

There is no duplicate values present in the data.

There is no constant column is present in Numerical as well as categoriacl data.

#### Data Preprocessing
Data underwent through various preprocessing techniques such as

Checking missing values - No missing values was present in the data.

outliers detection - Boxplot was used to detect outliers

Categorical Encoding - Typically, any structured dataset includes multiple columns – a combination of numerical as well as categorical variables. A machine can only understand the numbers. It cannot understand the text. That’s primarily the reason we need to convert categorical columns to numerical columns so that a machine learning algorithm understands it. This process is called categorical encoding.

Categorical Encoding - Label Encoding is a popular encoding technique for handling categorical variables. In this technique, each label is assigned a unique integer based on alphabetical ordering.

Data Scaling - Data has been scaled with the use of MinMax Scaler

Feature Importance - Feature importance has been done to find out the most important feature which affects the organization most.

#### Feature Selection
Dropping unique and constant feature: Dropping employee number because this is a constant column.

Checking Correlation: Checking correlation with the help of heat map, and we viewed that there was no highly correlated features in the dataset.

Heatmap: A heatmap is a graphical representation of data that uses a system of color-coding to represent different values.

##### Model Creation and Evaluation
Defining Dependant and Independant Features

Balancing the data: The data is imbalance, so we need to balance using SMOTE technique. SMOTE: SMOTE (synthetic minority oversampling technique) is one of the most commonly used oversampling methods to solve the imbalance problem. It aims to balance class distribution by randomly increasing minority class examples by replicating them. SMOTE synthesises new minority instances between existing minority instances.

Splitting Training And Testing Data: 75% data use for training & 25% data used for testing

Algorithm: A machine learning algorithm is the method by which the AI system conducts its task, generally predicting output values from given input data.

AIM: Create a sweet spot model (Low bias, Low variance)

HERE WE WILL BE EXPERIMENTING WITH SIX MACHINE LEARNING ALGORITHM

Logistic Regression

Decision Tree Classifier

Support Vector Machine

K-Nearest Neighbor

Random Forest Classifier

Gradient Boosting

But the best performing model to predict the performance rating of the employees are Best performing models to predict the performance of the employees are with accuracy scores are: Random Forest Classifier :- 97% Gradient Boosting :- 96% Decision Tree with best hyperparameter :- 95%

#### Challenges Faced
The Target feature had multiple output which clearly indicates that this is a multi classification task.Conversion of multi-class into binary class in order to perform algorithms.

Performing Exploratory Data Analysis.

Performed various Trial and Error such as handling of all outliers, handling partial outliers.

Selecting the best model for the given business case.
