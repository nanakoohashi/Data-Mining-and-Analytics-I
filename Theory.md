# Overview of Data Mining
Businesses want information about their costumers, products, services, competitors, business environment, and more, and data mining can help them find it.
- **Customers**: The aim of **customer relationship management (CRM)** is to understand th expectations of customers and anticipating their needs.
  - **CRM is composed of two main elements**:
    1. **Analytical CRM**
      - **Aim**: Extract, store, analyze and output the relevant information to provide a comprehensive, integrated view of a customer in the business, in order to understand his profile and needs more fully.
        - **Raw Marterial of Analytical CRM** = Data
        - **Components of Analytical CRM** = Data warehouse, data mart, multidimensional analysis (online analytical processing), data mining, reporting tools.
    2. **Operational CRM**
      - **Aim**: Managing the various channels (sales force, call centers, voice servers, interactive terminals, mobile telephones, internet, etc.) and marketing campaigns for the best implementation of the strategies indentified by the analytcial CRM.
      - Is based on the results of analytical CRM, but also supplies analytical CRM with data for analysis. Thus, there is a data 'loop' between operational and analytical CRM, reinforced by the fact that the multiplication of communication channels means that customer information of increasing richness and complexity has to be captured and analyzed. 
  - **Customer segmentation** involves looking at the behavior and developing a descriptive profile for your customers. These profiles are then used to provide prersonalized marketing programs and strategies that are appropriate for each group.
- **Competitors**: If you have more information about customers than your competitors, is that an advantage? How big of one?
- **Products/Services**: What kind of products are selling well? *e.g. Online shopping suggestions.*
- **Environment**: What are the market trends that affect your industry?
## Data mining
The combination of artificial intelligence (AI) and statistical analysis to discover information that is "hidden" in the data.
  - *Hidden* data includes:
    - Forecasting
    - Associations
    - Sequences
    - Classifications
    - Anomalies
    - Grouping/Clusters/Segments
  - **Types of data mining**:
    - **Descriptive (=Exploratory)**: Designed to bring out information that is present but burried in a mass of data
      - Clusters, groups, associations between different products or relief symptoms that you didn't initially see.
    - **Predictive**:  Designed to extrapolate new information based on present information, this new information being **qualitative (in the form of classification or scoring)** or **quantitative** (regression).
- A note on terminology. **Variable** is taken to mean any characteristic of an entity (person, organization, object, event, case, etc.) which can be expressed by a numerical value (a measurement) or a coded value (an attribute). The different possible values that a variable can take in the whole set of entities concerned are called the **categories** of the variable. The statistical entity that is studied is often called the **individual**, even if it is not a person. According to statistical usage, we may also use the term **observation**.
### Data Mining for one-to-one marketing
Data mining makes use of databases, or, increasingly, data warehouses, which store the profile of each customer, in other words the totality of his characteristics, and the totality of his past and present agreements and exchanges with the business. This global and historical knowledge of each customer enables the business to consider an individual approach, or ‘one-to-one marketing’, as in the case of a corner shop owner ‘who knows his customers and always offers them what suits them best’. The aim of this approach is to improve the customer's satisfaction, and consequently his loyalty, which is important because it is more expensive (by a factor of 3–10) to acquire a new customer than to retain an old one, and the development of consumer comparison skills has led to a faster customer turnover. 
### 10 Steps of Data Mining Study Development
#### 1. Define the aims
  - Define the target population - do you want prospects and customers, customers only or loyal customers only? All patients or only those patients who can be cured by the treatment under test?
  - Define the statistical entity to be studied (e.g. a person, a specific kind of household, a business, etc.)
  - Define some essential criteria and especially the phenomenon to be predicted.
  - Plan the project, deciding on the expected operational use of the information extracted and models produced.
  - Specify the expected results.
#### 2. List the existing data
- List the data that will be useful, accessible, exploitable, reliable, and sufficiently up-to-date and where they can be found.
- If the aim is to construct a predictive model, it will also be necessary to find a second type of data, namely the historical data on the phenomenon to be predicted.  
#### 3. Collect the data
- This step leads to the construction of the database that will be used for the construction of models. This *analysis base* is usually in the form of a table, having one record (row) for each statistical individual studied and one field (one column) for each variable relating to this individual.  
#### 4. Explore and prepare the data
- Check the origin of the data: Is the data reliable? Replace or remove incorrect data, extreme values, aberrant values, missing values.
- Create relevant indicators.
- Reduce the number of dimensions of the problem.
#### 5. Segment the population
- It may be necessary to segment the population into groups that are homogenous in relation to the aims of the study, in order to construct a specific model for each segment, before making a synthesis of the models. This method is called *stratification of models*. It can only be used where the volume of data is large enough for each segment to contain enough individuals of each category for prediction.  
#### 6. Draw up and validate the predictive models
- This step is the heart of the data mining activity, even if it is not the most time-consuming. It may take the form of the calculation of a score, or more generally a predictive model, for each segment produced in the preceding step, followed by verification of results in a test sample that is different from the learning sample. 
- It may also be concerned with detecting the profiles of customers, for example according to their consumption of products or their use of services of a business.  
#### 7. Deploy the models
- Involves the implementation of the data mining models in a computer system, before using the results for action (adapting procedures, targeting, etc.) and making them available for users (information on the workplace, etc.)  
#### 8. Train the model users
- Users must know the objective, the principles of the tools, how they work, their limits, the methods for using them (while pointing out that these are *decision support* tools, not tools for automatic decision making), what the tools will contribute (the most important point), and how the users' work patterns will change.  
#### 9. Monitor the models
- Whenever a new data mining application is brought into use, the results must be analyzed.  
#### 10. Enrich the models
When the results of the use of a first data mining model are measured, the model can be improved, as we have seen, either by adding independent variables that are not considered initially, or by using feedback from experience to determine the profiles to be predicted (e.g. 'purchaser/non-purchaser') if theses results were not available before.  
### Implementation of Data Mining
The main factors in the success of a project are:
1. Precise, substantial and realistic targets;
2. The richness and quality of the information collected;
3. The cooperation of the departmental and statistical specialists in the organization;
4. The relevance of the data mining techniques used;
5. Satisfactory output of the information generated and correct integration into the information system where appropriate;
6. Analysis of the results and feedback of experience from each application of data mining, to be used for the next application.

# Data Exploration and Preparation
## Types of Data
### Quantitative (=numerical)
- **Continuous**
  - Have possible values that cannot be counted and can only be described using intervals on the real number line. 
  - *e.g. length, height, salary*
- **Discrete**
  - Represent items that can be counted; they take on possible values that can be listed out; there is no continuum between values.
  - *e.g. number of items bought*
### Qualitative
Categorical data represent characteristics such as a person's gender, marital status, hometown, or types of movies they like. They may have numberical values (such as "1" indicating male and "2" indicating female), but those numbers don't have mathematical meaning.
- **Ordered (=Ordinal, Discrete)**
  - Falls into categories, but numbers placed on the categories have meaning (e.g. ratings, ranks).
  - *e.g. Low, medium, high*
- **Non-ordered (=Nominal)**
  - *e.g. Blue, white, orange etc.*
### Text
Uncoded texts, written in natural language:
  - *e.g. letters of complaint, reports, and press dispatches.*

## Exploring Data
### Univariate
Univariate means we are looking at one variable.
- One of the simplest ways to analyze data
- To describe a set of data, you can summarize it or describe the overall pattern. The best way to start seeing it is by literally looking at it. You can tell patterns, differences between groups, anomalies such as outliers or missing values by looking at graphs and charts.
- You can describe univariate data using numerical measurements, such as the mean, median, mode, standard deviation.
  - **Barchart**: Qualitative or Discrete Variable.
    - Frequency Table
  - **Histogram and Box Plot**: Continuous Variable.
  
### Exploring Data: What else to explore?
Data objects that don't follow the general behavior of other data:
- Aberrant values
- Misisng values
- Extreme values  
These might be considered noise or exceptions, but might also be used in fraud detection or might be a rare event.

## Tests of Normality
Many statistical procedures (including correlation, regression, t-tests, and analysis of variance) are based on the assumption that the data follow a normal distribution; that is, it is assumed that the populations from which the samples are taken are normally distributed. 
### Shapiro-Wilk (P-P) plot
In the Shapiro-Wilk test, the cumulative distribution of the data is shown on a normal probability scale, called a P-P (probability-probability) plot, where a normal distribution is shown by a straight line with a slope of 1. Thus the Shapiro-Wilk statistic is a way of measuring how far the graphic representation of the data deviates from the straight line.
### Kolmogorov-Smirnov
The Kolmogorov-Smirnov test involves measuring the maximum deviation *D* (in absolute terms) between the distribution function (cumulative density function) of the variable tested and the distribution function of a Gaussian variable (or, more generally, of any continuous variable whose distribution is to be compared with that of the observed variable). We then calculate the probability of obersving such a large value of *D* on the hypothesis H0 that the tested data come from a normal distribution. If this probability is below a given threshold of 0.05 ir 0.10 (a higher threshold can be used if the sample sizes are smaller), we reject H0 and conclude that the data do not come from a normal distribution.
### Anderson-Darling
This is most often used where a family of distributions are being tested, in which case the parameters of that family need to be estimated and account must be taken of this in adjusting either the test-statistic or its critical values.

## Homoscedascity
A formal requirement for some statistical analyses which is used to compare the means of two or more groups.  
- Literally means 'having the same scatter/variance' and indicates having data values that are scattered, or spread out, to about the same extent.
- *e.g. Imagine that you want to use family income to predict luxury spending. At the lower income levels, you won't see much variance because they don't have much to spend. However, when you get to the higher income levels, families vary greatly in their luxury spending. Some people like to save; some are spenders. In this case, you don't have homoscedacity (you have heteroscedacity), and your regression model could be impacted.*
- Tests for homoscedacity include:
  - Levine (best - has low sensitivity to non-normality)
  - Bartlett (best if the distribution is normal)
  - Fisher (the least robust if normailty is not preent)
  
## Bivariate Analysis
- **Bivariate** = two variables
- With bivariate data you have two sets of related data you want to compare.
  - Incompatibilities between variables;
  - Links between the dependent ('target') variable and the independent variables and their interactions, in order to eliminate the variables having no effect on the dependent variable;
  - Links between the independent variables, which must be avoided in some methods, such as linear and logisitic regression.
- *e.g. A bike shop might want to measure how many bicyclists come in on warm weather days vs. cold weather days.*
- You might have **two discrete variables**: such as when measuring the link between gender and smoking.
  - Tests:
    - Cramer's V
    - Chi-Squared
- You might have **one discrete and one continuous variable**, as when measuring dosage of a medicine and recovery time. 
  - Tests:
    - Parametric ANOVA test
      - Requires normality/homoscedacity assumption
    - Non-parametric approaches
      - Wilcoxon-Mann-Whitney (2 groups)
      - Kruskal-Wallis (>2 groups)
## Data Preparation: Transforming Variables
Why do we need to prepare data?
- In the real world applications data can be inconsistent, incomplete, and/or noisy
  - Data entry or data collection problems
  - Discrepancy in naming conventions
  - Duplicated records
  - Incomplete or missing data
  - Contradictions in data
  - Decisions are based on the data; bad data=bad decisions
## Transforming Variables: Data Normalilization 
**Goal of Data Normalization**: Make the variables proportional to one another.
  - *e.g. if one variable is 50x larger than another (on average), you may want your variables to be approximately equivalent in the model. That way, the coefficients will reflect meaningful relative activity between each variable (i.e. a possible coefficient will mean that the variable acts positively towards the objective function, and vice versa, plus a large coefficient versus a small  coefficient willl reflect the degree to which that variable influences the objective function.
  - Normalization of a continuous variable is done by transforming the variable with a mathematical function, which compresses its distribtuion, brings it closer to a normal distribtuion, and, if necessary, decreases its heteroscedasticity and increases its discriminating power in a linear model.
## Transforming Variables: Data Discretization
- **Discretization**: process of converting continuous data into a typically small number of finite values (e.g. high, medium, low). 
- The variation in the original data is maintained in the discretized dataset.
- Discretization is a necessary precursor to data mining and is accomplished by assigning each value in a dataset to a bin. 
- Data ranges = bin boundaries
### Tips for creating bins:
- Avoid too many differences in classese between variables
- Avoid too many classes for a variable
- Avoid classes too small (4-5 classes is good).
## Variable Interaction
One phenomenon commonly encountered in the real world is that the simultaneous action of two variables is not the sum of the independent actions of the variables = 'interactions' between the variables.
  - *e.g. When looking at gender and smoking, is age also a consideration? Are older females more likely to smoke?*
  - This step of detecting the interactions has to preformed by some models such as linear models (linear discriminant analysis or logistic regression), which are additive.
## Collinearity
- **Definition**: Correlation among the predictors in a multiple regression.
- Because of this "redundancy", collinearity confuses the effects of the predictors.
- *e.g. if height and weight are both used to predict something (e.g. intelligence), your results will be skewed because height and weight are related (generally because the taller someone is, the more he weighs related to someone shorter).*
## Random Sampling
- **Sampling**: indispensable procedure in statistics and data mining, especially in prediction and classification, where most algorithms use a *training sample* for developing the model and a *test sample* for validating the model, or multiple samples for cross-tabulated validation.
- Sampling is required for the development of a predictive model, if only for the creation of the training and test samples for optimizing the selection of the independent variables.
### Four methods of sampling
#### 1. Simple Random Sampling
Involves drawing *n* individuals at random without replacement from a populatoin of *N*, each individual having a probability of 1/*N* of being drawn.
#### 2. System Sampling
The individuals are drawn not at random, but in a regular way. If we carry out a '1/100' sampling, we take the first individual, then the 101st, then the 201st, and so on. We must pay attention to the cyclical data with this form of sampling: if we use customer numbers, the hundreds number may be a family number, and if we take one customer in every hundred, we will never choose two individuals in the same family. However, this sampling mode can also provide a degree of comprehensiveness.
#### 3. Stratified Sampling
Here, we divide the populuation, *e.g. by divinding the customers into age ranges*, and then draw customers at random from each stratum to obtain a sub-sample for each stratum; we can then bring all these sub-samples together.
- **Proportional Stratified Sampling**: the relative size of each sub-sample is equal to the relative size of the corresponding division: *e.g. if 30% of the customers in the population are aged >60, then 30% of any stratified sample by age must be aged >60.
- **Nonproportional Stratified Sampling**: It amy be useful to carry out a non-proportional stratified sampling procedure to take itno account the variability of the phenomena studied in each stratum: thus we can underrpresent the strata in which the variability is low (where the interesting information is concentrated in a few individuals) and overrepresent the strata in which the variability is high (which require a larger number of individuals to establish the information).
#### 4. Cluster Sampling
Drawing favmilies of individuals (the 'clusters') at random and choosing all the individuals in each cluster, thus being know as a **census**.
- We may, for example, choose certain urban districts at random and then ask questions of all the customers from these districts. Or we can choose a family name at random and then carry out a census of all the customers whose family name starts with the letter drawn at random.
## Linear Regression Assumptions
### 1. Linearity
### 2. Independence of Errors
  - Residuals should not following a pattern.
  - Errors (residuals) should be random.
### 3. Homoscedasticity
  - Residuals should not get larger (funnel shaped) as you go along the x-axis.
  - If residuals are plotted on a separate graph, they should have a slope of 0 (horizontal line).
    - Heteroscedastic residuals plotted on a separate graph should have a postive slope.
### 4. Normality of Error Distribution
  - Distance from residuals to linear line should be normally distributed (i.e. most residuals are close to the predicted line, with very few outliers). 
# Statistical Tools, Techniques and Methods: Commercial Data Types
## Evolution from business data to business information
1. What happened?
  - *e.g. What was my total revenue in the last five years?*
2. Why did it happen?
  - *e.g. Why were sales higher in the Western region than the Eastern region last quarter?*
3. What will happen?
  - *e.g. What's likely to happen to Los Angeles unit sales next month? Why?*
4. What is the best that could happen? (optimization)
  - *e.g. What ad campaign to which new market segment will likely lead to the highest sales volue?*
## Types of Data
There are several common types of data that are used in commercial sectors.
### 1. Transactional Data
- Where? (geographical locations, businesses where the transactions took place, internet, etc.)
- When? (frequency and recency of the transations)
- How? (method of payment)
- How much? (number and value of transations)
- What? (what has been purchased)
### 2. Product Data
Information can be collected on different products (numbers, types, options, prices, date of purchase or subscription, date and reason for cancellation or return of products, mean product life or expiry date, payment date and method, discount granted to the customer, and profit margin on this product for the business, etc.)
### 3. Customer Data
Data on customers include:
- **Lifetimes**: *i.e. age, lifetime as a customer of the business, length of time in present job.*
- **Relational, Attitudinal, and Psychographic Data**: *i.e. responses to marketing campaigns and offers, loyalty, satisfaction, lifestyle, personality.*
- **Sociodemographic Data**: *i.e. sex, education, occupation, income, geographical information.*
- **Channel**: *i.e. through which contact, orders, and delivery came through.*
### 4. Geodemographic Data
Environmental and geodemographic includes: competition, population, working population, customer population, unemployment rates, economic potential, product ownership rates, etc., in the area of residence of the customer or prospect, etc.  
- The existence of these data has led to the emergence of geomarketing which basically assumes that the customer's potential for the business will be roughly equal to the difference between the 'shopping basket' of consumers in his area and what he has purchased already.
#### More about Geographic data
- Not relating to individuals, but to geographic environment
- Modeling and analysis of all factors between customer's residence and mode of consumption (Franck Bleuzen)
- Place of residence in terms of economics, sociodemographics, housing and competition
### Other Data Types (technical)
In addition to the main types of data seen on the previous slide, there is also technical data which is not used within a data mining analysis but is used to determine whether individuals are included in the analysis base. Technical data includes:
- Type of customer
- Non-acceptance of direct marketing
- Bad payer status
- Status as employee of the business
- Title, surname, forename
### Profitability Data
- Special type of data
- It is the difference between the profits to the business from a customer, segment, or market, etc., and the costs incurred, namely the acquisition and structural costs, commercial costs, operation processing costs and the cost of finance
- Profitability to a business from a customer or business segment
  - Determine the most profitable customers
  - Hard to measure precisely
  - Important measure is the **lifetime value** (LTV)
    - Net present value of profitability of customer.
## Data Used in Business Sectors
- Four sectors
  - Banking
  - Insurance
  - Telephone
  - Mail Order
# Software Comparison
## Software programs
1. **SAS**: Market leader for commercial applications. The software offers many statistical functions, has a good user interface for people to learn quickly and provides technical support. However, it ends up being the most expensive option and is not upgraded as rapidly as some of the others.
2. **R**: Open source counterpart of SAS, which has traditionally been used in academics and research. Because of its open source nature, updates get released quickly. There is a lot of documentation available over the internet, and it is a very cost-effect option.
3. **Python**: Originally a source scripting language, Python is growing very rapidly. Today, it has libraries and functions for almost any statistical operation or model building and has become very strong in operations on structured data.
4. **SPSS**: Data mining software produced by IBM. It is common among some companies (but less so than either SAS or R). It works with large data systems. SPSS will not be covered in this course, although there are many resources online, if you would to become more familiar with it.
# Data Mining Methods
## Data Mining Techniques
### 1. Descriptive Methods
Designed to bring out information that is present but buried in a mass of data (as in the case of automatic clusering of individuals and searches for associations between products or medicines).
- **Purpose**: Summarization for insight in performance
  - *e.g. number of sales, social media posts, followers, or average amount of sales, etc. 
### 2. Predictive Methods
Designed to extrapolate new information based on the present information, this new information being qualitative (in the form of classification or scoring) or quantitative (regression).
- **Purpose**: Use statstical models and forecasting to allow you to predict what might happen in the future. They combine the past data to identify patterns and models.
  - *e.g. forecasting inventory needs, identifying trends in sales activities, predicting what customers will buy which items.
## Descriptive Methods (= Unsupervised Methods)
Do not predict a target value (*i.e. there is not a dependent variable*) but focus more on the structure, relationships, and interconnectedness of the data. Descriptive methods reduce, group, and summarize data. *e.g. you might want to identify the web pages that are accessed together*.
### 1. Cluster Analysis
Given a set of data points, each havign a set of attributes and a similarity measure among them, find clusters such that the data points in one cluster are more similar to one another and less similar to those in separate clusters.
- *e.g. Consider a bookstore with different areas for the types of books: History, Self-Help, Romance, Mystery & Crime etc. The books in each of these clusters are more similar to each other than they are to otther clusters*
### 2. PCA
Imagine that you have a lot of information about your customers -- you might know their  gender, the  days of the week they typically shop, the products they buy, the frequency with which they buy certain items, the amount spent on the average trip, etc. You could have so many variables that it would cloud the picture -- you might not be able to see any patterns. Principal Component Analysis (PCA) can help you identify which variables are important so you can compress the data by reducing the number of dimensions. 
### Association Analysis (= Market Basket Analysis)
Association Analysis is also called Market Basket Analysis. In a given set of records, each will contain a number of items. Association Analysis allows you to determine the degree to which the items tend to be associated with one another. 
- *e.g. people who buy hamburger buns will also likely buy ketchup and mustard and hamburger meat. You can associate items together and create rules.*
## Predictive Methods (= Supervised Methods)
The objective of this method is to predict the value for a specific attribute (a dependent variable) based on the value of other attributes. 
- *e.g. You might want to judge how a high school student will perform in college based on school grades, extracurricular activities, and standardized test scores. *
- Grouped as either prediction techniques or classification techniques:
- **Two important features critical to the classification of a data mining technique as a supervised learning method**:
  1. The use of previously observed events, typically referred to as a target variable data.
  2. The description of the target variable in terms of a set of explanatory variables.
### Prediction Techniques
  - Dependent variable is continuous.
#### 1. Linear Regression
A common way of estimating the relationship between one or more input variables and a continuous target variable.
- Assumes that the relationship between a continuous target variable and its corresponding inputs is linear - *i.e. best described by a straight line*. The fitting of a linear regression model involves the estimation of parameter estimates of "weights" that describes the influence of each input on the target variable value. These weights can also be used to predict the value of a new events.
#### 2. Decision Trees
Decision trees are akin to regression models in the way they fit a target variable to input variables, but does so one input at a time - first finding the split in a single variable that best discriminates between values of the target variables. The decision tree then continues to evaluate the remaining variables for the one that best further discriminates between target variable values, and so on until some criteria is reached at which the decision tree stops evaluating variables. Decision trees are popular in practice because they tend to be computationally straighforward and provide and intuitive application to new data for predicitve use.
- *Note: if used to apply to existing data and not to new data, the Decision Tree method would be considered a Classification Technique.*
#### 3. SVM
A support vector machine (SVM) is associated with algorithms that can, given a set of training examples, build a model that assigns new examples into one category or another.
#### 4. Neural Networks
Neural networks do not typically reflect a linear relationship between a target and some set of inputs. Neural network models emulate aspects of human cognition and are flexible with regards to their ability to fit a target to non-linear relationships, and can approximate functions that depend on a large number of inputs. However, neural networks may become computationally intensive.
- *Note: if used to apply to existing data and not to new data, the Neural Network method would be considered a Classification Technique.*
### Classification Techniques
  - Dependent variable is binary or discrete.
#### 1. LDA
- **Purpose**: Classifies (or discriminates) a qualitative outcome based on a set of inputs (usually quantitative).
- *e.g. you might want to classify people based on a set of features - credit officers might want to determine if isomeone is a good risk or a bad risk (discriminate categories) based on different features, such as income, credit scores, etc.*
#### 2. Logistic Regression
- **Purpose**: Describes data and explains relationship between one dependent binary variable and one or more interval or ratio scale independent variables.
- *e.g. you might want to know whether body weight and b ody fat percentage influence the occurence of diabetes (yes or no) in a person, for instance.*
#### 3. Naive Bayes Classifier
Naive Bayes is an algorithm that uses a set of training data to construct a model that can classify new data points.
- *e.g. consider that your training data consist of red, round, apples; yellow, oblong bananas. If you have new object that is red, the probability is greater that it is an apple.*
