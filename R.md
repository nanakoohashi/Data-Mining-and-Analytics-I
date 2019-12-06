# R
## Basic Tests
### Summary statistics
Minimum, 1st Quartile, Median, Mean, 3rd Quartile, Maximum, NA's.
 - **Code**: summary(*imported .csv file* $ *name of column you want to summarize*)
 - e.g. summary(normalization$income)
### Quantile
95% and 99% Quantile
- **Code**: quantile(*imported .csv file* $ *name of column*, na.rm = TRUE, probs = c(0.95,0.99))
- e.g. quantile(normalization$income, na.rm = TRUE, probs = c(0.95,0.99))
### Histogram
Graph histogram
- **Code**: hist(*imported .csv file* $ *name of column*)
- e.g. hist(normalization$income)
### Log Transformation
To transform the data to a form where we will see a more normal distribution if data is skewed from the histogram code.
- **Code**: *imported .csv file* $ *name of new column* <- log(*imported .csv file* $ *name of column*)
- e.g. normalization$log_income <- log(normalization$income)
- You can now use hist(normalization$log_income) to see the log version.
- If this does not correct the skew,  you can do a square root transformation.
### Square Root Transformation
To transform the data to more closely resemble a normal distribution if the log transformation did not correct the issue.
- **Code**: *imported .csv file* $ *sqrootincome* <- sqrt(*imported .csv file* $ *income*)
- e.g. normalization$sqrootincome <- sqrt(normalization$income)
- You can now use hist(normalization$sqrootincome) to see the square root version.
## Normality Tests
### Shaprito-Wilk Test
- **Code**: Shapiro.test(*imported .csv file* $ *name of column*)
- e.g. Shapiro.test(normalization$income)
## Tests for Categorical Variables
Better understood using tables, rather than summary statistics.
### One-Way Tables
- **Code**: table(*name of .csv file* $ *name of column*)
- e.g. table(chd$CHD)
- e.g. table(chd$CLASS)
#### Check the relationship between the two categorical variables 
First install "gmodels" package
- install.packages("gmodels")
- Tick the gmodels box in "packages" tab.
- **Code**: CrossTable(x = *name of .csv file* $ *name of column1*, y = *name of .csv file* $ *name of column2*)
- e.g. CrossTable(x = chd$CLASS,y=chd$CHD)
### Chi-Square Test to determine relationship beteen variables
- **Code**: CrossTable(x = *name of .csv file* 
- e.g. CrossTable(x = chd$CLASS,y=chd$CHD, chisq = TRUE)
## Exploring Multivariate Relationships
## Using Scatterplots to Explore Relationships
- **Code**: predictors <-as.matrix(*name of .csv file* [,-1]) 
 - pairs(*name of .csv file*)
- e.g. predictors <-as.matrix(heating[,-1])
 - pairs(predictors)
## Pearson's Correlation to Explore Relationships Between Variables
- **Code**: cor(*name of .csv file*)
- e.g. cor(predictors)
- Any value close to 1 = high correlation
- If value close to 1 continue to cor.test() command for p-value
### Cor.test() for p-value
- **Code**: cor.test(*name of .csv file* $ *column1*, *name of .csv file* $ *column2*)
  - cor.test(*name of .csv file* $ *column3*, *name of .csv file* $ *column2*)
  - cor.test(*name of .csv file* $ *column1*, *name of .csv file* $ *column3*)
- e.g. cor.test(heating$temperature, heating$insulation)
  - cor.test(heating$othervariable, heating$insulation)
  - cor.test(heating$temperature, heating$othervariable)

