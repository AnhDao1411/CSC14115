# New York City Taxi Trip Duration

## Problem Statement

### Overview
 @AD
 
### Input and Output Data description
@NL

### Evaluation Metric
- **Root Mean Squared Logarithmic Error** (RMSLE) is the metric was used to assess the result of this contest.

$$\epsilon = \sqrt{\frac{1}{n}\sum^{n}_{i=1}(log(p_i + 1) -log(a_i + 1)) ^2}$$

* With respect to:
    * $$\epsilon$$: RMSLE score
    * n: the number of records (trip duration's observations) in the dataset
    * $$p_i$$: the prediction of trip duration
    * $$a_i$$: the actual value of trip duration
    * log(x): natural logarithm (base is e)

* **The smaller the RMSLE value is, the better the model**.
