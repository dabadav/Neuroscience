
## Wilson-Cowan

### Equation

$$\tau_E \frac{dr_I^E}{dt} = -r_I^E(t)+F \left[c_{EE} r_I^E(t) - c_{EI,i}(t)r_i^I(t) + C\sum_{j=1}^NW_{ij}r^E_i(t-\tau_{ij}) + \xi(t) + P\right]$$

$$\tau_I \frac{dr_i^I(t)}{dt} = -r^I_i(t) + F \left[ C_{IE} r^E_i (t) + \xi(t)\right]$$


### Requirements
```
numpy==1.23.5
numba==0.56.4
pymatreader==0.0.30
scipy==1.10.1
notebook==6.5.2
```

### Activation function
$$ F(x) = \frac{max_S}{1 + e^{-(\frac{x - \mu}{\sigma})}} $$

where:
- $max_S$ is the maximum value of the sigmoid
- $\mu$ is the midpoint of the sigmoid, 
- $\sigma$ is the slope of the sigmoid
- $maxS$ is the maximum value of the sigmoid

### Parameters
Global parameters such are normally tuned:
`C` = 0.1
`md` = 4 ms
`rho` = 0.22
Pre-tuned parameters:
`sd_noise` = 0.01
`C_EE`
`C_IE`
`C_EI`
Recording parameters:
`dt_save = 2 ms` 
`dt = 0.2 ms`

### VSI Simulation
---
#### Parcellation
Mask according to the Allen Brain Atlas

#### Connectome
https://www.nature.com/articles/nature13186 

#### Resting state data