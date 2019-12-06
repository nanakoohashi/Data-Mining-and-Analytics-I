# Data-Mining-and-Analytics-I
## R
### Summary statistics
Minimum, 1st Quartile, Median, Mean, 3rd Quartile, Maximum, NA's.
 - **Code**: summary(*imported .csv file* $ *name of column you want to summarize*)
 - e.g. summary(normalization$income)
### Quantile
95% and 99% Quantile
- **Code**: quantile(*imported .csv file* $ *name of column*, na.rm = TRUE, probs = c(0.95,0.99))
- e.g. quantile(normalization$income, na.rm = TRUE, probs = c(0.95,0.99))
