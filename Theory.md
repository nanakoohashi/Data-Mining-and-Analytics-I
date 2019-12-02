# Overview of Data Mining
Businesses want information about their costumers, products, services, competitors, business environment, and more, and data mining can help them find it.
- **Customers**: The aim of **customer relationship management (CRM)** is to understand th expectations of customers and anticipating their needs.
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
### 10 Steps of Data Mining Study Development
1. Define the aims
  - Define the target population - do you want prospects and customers, customers only or loyal customers only? All patients or only those patients who can be cured by the treatment under test?
  - Define the statistical entity to be studied (e.g. a person, a specific kind of household, a business, etc.)
  - Define some essential criteria and especially the phenomenon to be predicted.
  - Plan the project, deciding on the expected operational use of the information extracted and models produced.
  - Specify the expected results
2. List the existing data
- List the data that will be useful, accessible, exploitable, reliable, and sufficiently up-to-date and where they can be found.
- If the aim is to construct a predictive model, it will also be necessary to find a second type of data, namely the historical data on the phenomenon to be predicted.
3. Collect the data
- This step leads to the construction of the database that will be used for the construction of models. This *analysis base* is usually in the form of a table, having one record (row) for each statistical individual studied and one field (one column) for each variable relating to this individual.
4. Explore and prepare the data
- Check the origin of the data: Is the data reliable? Replace or  remove incorrect data, extreme values, aberrant values, missing values.
- Create relevant indicators.
- Reduce the number of dimensions of the problem.
5. Segment the population
- It may be necessary to segment the population into groups that are homogenous in relation to the aims of the study, in order to construct a specific model for each segment, before making a synthesis of the models. This method is called *stratification of models*. It can only be used where the volume of data is large enough for each segment to contain enough individuals of each category for prediction.
6. Draw up and validate the predictive models
- This step is the heart of the data mining activity, even if it is not the most time-consuming. It may take the form of the calculation of a score, or more generally a predictive model, for each segment produced in the preceding step, followed by verification of results in a test sample that is different from the learning sample. 
- It may also be concerned with detecting the profiles of customers, for example according to their consumption of products or their use of services of a business.
7. Deploy the models
- Involves the implementation of the data mining models in a computer system, before using the results for action (adapting procedures, targeting, etc.) and making them available for users (information on the workplace, etc.)
8. Train the model users
- Users must know the objective, the principles of the tools, how they work, their limits, the methods for using them (while pointing out that these are *decision support* tools, not tools for automatic decision making), what the tools will contribute (the most important point), and how the users' work patterns will change.
9. Monitor the models
- Whenever a new data mining application is brought into use, the results must be analyzed.
10. Enrich the models
When the results of the use of a first data mining model are measured, the model can be improved, as we have seen, either by adding independent variables that are not considered initially, or by using feedback from experience to determine the profiles to be predicted (e.g. 'purchaser/non-purchaser') if theses results were not available before.
