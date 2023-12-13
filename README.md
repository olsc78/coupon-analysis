# coupon-analysis
Analyzing the acceptance rates from cohorts of drivers exposed to various coupons. Data from a survey on Amazon Mechanical Turk.

## Dataset
- The CSV dataset can be found here: data/coupon.csv

## Notebook and Repository
- The analysis of the data supporting the findings can be found in the Jupyter Notebook "coupon-analysis-olivierschott.ipynb"
- Git Repository is located at https://github.com/olsc78/coupon-analysis.git

## Summary of findings

### Data 
- Missing data were found and cleaned. With 99% of NaN value, the entire 'car' column was dropped. Other columns had data missing representing less than 2% of the entries. They were cleaned either by replacing with the values represented the most, or simpply by dropping the rows. See notebook.

### Coupons for bars
In general, 60% of bar coupons were accepted, but some interesting features were found to create cohorts with significantly higher acceptance rates (around 70%):
- Age has a key influence on acceptance rate: drivers between 21 and 30 years old have a higher acceptance rate.
- Frequency of monthly visits to a bar is a key factor: acceptance will increase significantly as soon as the respondent visits a bar at least once a month.
- Marital Status and occupation have no influence on whether the driver will or will not accept the coupon. Indeed, the acceptance rates are exactly the same in questions 5 and 6.
- Having a kid as a passenger tends to slightly refrain the driver from accepting the coupon but the influence is limited.
- Frequency of going to a restaurant has no positive impact on accepting bar coupons

### Coupons for restaurant between $20 and $50
In general, 55% of restaurant coupons were accepted, but here again specific features could increase acceptance rate significantly (in the range 62% - 76%):
- Frequency of monthly visits to a restaurant is a key factor: drivers going at least once a month tend to accept coupons more
- Having the driver's partner as passanger increase the acceptance rate significantly
- Not surprisingly, coupon for a restaurant resonates less with divorced or widowed drivers
- The time of the day where the coupon is proposed and the nature of the coupon (when it expires) have an influence over triggering the driver to accept the coupon: proposing coupons valid for 24 hours at 10am or 2pm is recommended
- Proposing a coupon on sunny/warm day will also increase the average acceptance rate
- The gender, as well as whether the restaurant is in the same direction or not, do not significantly influence the acceptance 
