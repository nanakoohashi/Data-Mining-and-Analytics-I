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
### Quantitative
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
  - ** Histogram and Box Plot**: Continuous Variable.
  
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
- *e.g. Imagine that you want to use family income to predict luxury spending. At the lower income levels, you won't see much variance because they don't have much to spend. However, when you get to the higher income levels, families vary greatly in their luxury spending. Some people like to save; some are spenders. In this case, you don't have homoscedacity (you have heteroscedacity), and your regression model could be impacted.
- Tests for homoscedacity include:
  - Levine (best)
  - Bartlett
  - Fisher
  
## Bivariate Analysis
- **Bivariate** = two variables
- With bivariate data you have two sets of related data you want to compare.
- *e.g. A bike shop might want to measure how many bicyclists come in on warm weather days vs. cold weather days.
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
