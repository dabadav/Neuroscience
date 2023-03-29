## VSDI Data
---
Data in the form of a numpy.ndarray from each session
```python
vsdi # (time, x, y)
```

## Preprocessing
---
**1. Motion correction matlab preprocessing**
- Motion correction applied to frames that are shifted respect to the others
- Ratiometric merge between both camera devices
- High-pass filter >0.5Hz to get rid of hemodynamic noise in the data
**2. Outlier correction**
A correction has been applied to the vsdi outlier frames by imputating the mean from the neighbour frames.
**3. Hemodynamics cleaning**
Component analysis:
- *PCA:* data is transformed through PCA, and Principal Components capturing hemodynamic movement, the ones presenting bimodal distribution of the timecourse are removed before projecting data to original space.
- *PCA-ICA:* feed the data through PCA, ICA pipeline and identify bimodality of timecourse to remove this hemodynamic noise related components
- *DMD*: another approach used by federico student

## Correlation with behavioural data
***
Timestamp of `Lick`, `CS+`, `CS-` during the session are stored in the form of a dictionary. From this data `Reward` timestamps can also be obtained.

**1. GLMs are used to observe the interaction between behavioural predictors and neural activity**

