# End-to-end-case-analysis-on-perception-of-consumers-towards-Biocon-Pharmaceuticals

## Topic of study:

Biocon Pharmaceuticals Ltd is a subsidiary or division of Biocon Limited that specifically deals with the pharmaceutical aspect of the business. It plays a significant role in the development, manufacturing, and distribution of pharmaceutical products. This includes the production of generic medicines, biosimilars (biological products similar to existing biologics), and other pharmaceutical formulations. 

This study aims to conduct the survey and a series of analysis to understand the consumer perception towards the Biocon Pharmaceutical Ltd. products.

## Executive Summary:
The exploratory survey on consumer perception towards Biocon Pharmaceuticals Ltd. is conducted on a set of people belonging to Karnataka region in order to understand their
perception and preference towards the pharmaceuticals of Biocon company. This gives insights into the brand loyalty, choice and preference and spending habits of the consumers
towards the product. There are around 50 respondents to this survey.

This study comprises of the end to end analysis involving collection of the real time data, performing univariate and bivariate Analysis, Exploratory Data Analysis(EDA), Data
preprocessing, Model building and result interpretation using various models.

## Data collection and data methodology:
The data is collected from various respondents through the Google form. It involves several questions such as Age, Gender, Occupation, Income levels, Consumer awareness about the
brand, their perception and spendings/month etc. The google form is as shown below.

## Questionnaire:

1. Name
   
2. Gender
   
   Male

   Female

3. Age
   
   18-24

   25-34

   35-44

   45-55

   Above 55

4. Occupation*
   
   Student

   Employee

   Business

   Other:

5. Annual income(in lakhs)*
   
   Below 2.5

   2.5-5

   5-10

   Above 10

6. Have you heard about Biocon Ltd. company?*
   
   Yes

   No

7. Rate on the scale of 1 to 5 (1= Strongly disagree, 2= Disagree, 3= Neutral, 4= Agree,
5=Strongly Agree)

   a) Biocon Pharmaceuticals is a reputable and trustworthy company in the
pharmaceutical industry.

   b) If you have purchased Biocon products, do you with agree with the quality and
effectiveness of the products?

   c) Would you consider choosing Biocon Pharmaceuticals' products over those of
other pharmaceutical companies?

   d) Does Biocon Pharmaceuticals meet your expectations?

8. Rate on the scale of 1 to 5 (1= Most unlikely, 2= Unlikely, 3= Neutral, 4= Likely, 5=
Most Likely)

   a) Would you recommend Biocon Pharmaceuticals to others based your
experiences?

   b) Do you actively seek out information about new products or developments from
Biocon Pharmaceuticals?

9. Would you recommend Biocon Pharmaceuticals to others?*

   Yes

   No

10. How much do you spend on products from Biocon pharmaceuticals?*

## Data methodology:

It involves

1. Univariate analysis.

2. Bivariate analysis.

3. Exploratory Data Analysis.

4. Data Preprocessing.

5. Model Building.

6. Interpretation of results.

## Data Analysis

### Data preprocessing:

The data that is obtained from the Google form is an inconsistent data. It has missing values, datatypes are not the same and some have special characters. In order to remove
inconsistency, data preprocessing is done using Excel. The preprocessed data now appears as shown in the diagram below.






## Exploratory Data Analysis:
EDA is carried out on the collected data to get the summary statistics and visualizations in order to analyze the main characteristics of the data to gain insights. This is carried out using
Python.

### Univariate analysis using JMP:





Interpretation: It can be inferred that, 71% of the respondents are students while 28% of the
respondents are male.


Interpretation: It can be inferred that, 71% of the respondents are students while 28% of the
respondents are employees.


Interpretation: It can be inferred that, the range of income lies between Rs.45000 to
Rs.1200000.


Interpretation: It can be inferred that, Bicon Pharceuticals Ltd. has been able to build a
reputation and gain a trust of 4 on the scale of 5.


Interpretation: It can be inferred that customers are satisfied with 3.6 rating with the Bicon
Pharceuticals Ltds. quality on the scale of 5.


Interpretation: It can be inferred that customers would prefer the Bicon Pharceuticals Ltd.
product 3.7 times than the other companies on a scale of 5.


Interpretation: It can be inferred that Bicon Pharceuticals Ltds. is able to meet the
expectations of the consumers at 3.7 rating on the scale of 5.


Interpretation: It can be inferred that customers are updated with the latest Bicon
Pharceuticals Ltds. information on a rating of 3.2 out of 5.


Interpretation: It can be inferred that 73% of the customers would recommend Biocon
products to others while 26% of them would not recommend.


Interpretation: It can be inferred that customers spend on an average Rs.524 on monthly basis
on Bicon Pharceuticals Ltd. products.


### Bivariate Analysis:
Using Python
Firstly, the libraries are imported in order to carry out the steps.


Then the .csv file is imported using the following code.


For quantitative data:
Pairwise Plot
The pairwise plot below gives the relationship between different variables showing the
distribution of each variable.


For Categorical data(Count plots)
Gender:


Occupation:


Recommendation:


## Data Reduction Methods: (Using JMP)

From the factor loading, it is seen that there are two factors that can be considered. These can be divided into two clusters. Based on the Quality and Expectations, the customers are named
as ‘Satisfactiory Customers’, based on Information updates and Suggestions, customers are named as ‘Engaged Customers’.
Cluster 1: Satisfactory customers
Cluster 2: Engaged customers


We now go for correlation matrix:

We can visualize the correlation matrix using heatmap as follows:

From the above heatmap, it can inferred that Annual Income has the problem of multicollinearity as its value is above 0.6.

### Cross Tabulation:

#### Marginal probability:

#### Conditional probability:

It can be inferred that, 39% of male are Employees and 19% of female are Employees among the 28% of totally employed respondents.

#### Joint probablity:

It can be inferred that, of the total number of employed respondents, 36% of them are female and 64% of them are male.

## Model building and result analysis:

The dataset is divided into Training and Testing data as follows. For this, the libraries essential for performing Train-test split are imported.

### Train test split:

The dummy variables for the categorical data such as Gender and Occupation are created.

The LabelEncoder is used to encode the dependent variable ‘Recommendation’.

Standardization:

#### Simple Linear Regression:

It can be inferred that 45% of variation in recommendation of Biocon pharma products is explained by several other factors.

#### Logistic Regression:

Precision:

For class 0: Precision is 1.00, indicating that when the model predicts class 0, it is correct all
the time.

For class 1: Precision is 0.78, indicating that when the model predicts class 1, it is correct
78% of the time.


Recall:

For class 0: Recall is 0.33, indicating that the model correctly identifies only 33% of the
instances belonging to class 0.

For class 1: Recall is 1.00, indicating that the model correctly identifies all instances
belonging to class 1.


F1 Score:

For class 0: F1-score is 0.50, which is the harmonic mean of precision and recall for class 0.

For class 1: F1-score is 0.88, which is the harmonic mean of precision and recall for class 1.


Support:

For class 0: There are 3 instances of class 0 in the dataset.

For class 1: There are 7 instances of class 1 in the dataset.


Accuracy: The overall accuracy of the model is 0.80, meaning it correctly predicts 80% of the
instances in the dataset.

Mean Average:

Macro-average F1-score: 0.69
Weighted-average F1-score: 0.76

