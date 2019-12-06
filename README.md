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
