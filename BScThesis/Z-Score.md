2023-02-24 11:34
Status: #idea 
Tags: #z-score #statistics

## How to Calculate Z-Scores in Python ( scipy.stats as stats)

>[!info] Z-Score 
>Tells us **how many standard deviations away a value is from the mean.** 

We use the following formula to calculate a z-score:
$$z = (X – μ) / σ$$

where:

- X is a single raw data value  
- μ is the population mean  
- σ is the population standard deviation

---

This tutorial explains how to calculate z-scores for raw data values in Python.

**How to Calculate Z-Scores in Python**

We can calculate z-scores in Python using scipy.stats.zscore, which uses the following syntax:

```python
scipy.stats.zscore(a, axis=0, ddof=0, nan_policy=’propagate’)
```

where:
- a: an array like object containing data  
- axis: the axis along which to calculate the z-scores. Default is 0.  
- ddof: degrees of freedom correction in the calculation of the standard deviation. Default is 0.  
- nan_policy: how to handle when input contains nan. Default is propagate, which returns nan. ‘raise’ throws an error and ‘omit’ performs calculations ignoring nan values.  

---
## References
https://www.kaggle.com/general/2107262
