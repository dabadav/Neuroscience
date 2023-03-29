2023-02-20 12:22
Status: #idea 
Tags: #dynamics #criticality #metastability

## Synchrony and Metastability

>[!info] **Kuramoto order parameter (KOP)**
> Represents the **degree of synchrony among a set of coupled oscillators** at a given point in time. The KOP can be calculated as:

![[Pasted image 20230220134247.png]]

- $𝜃_𝑛(𝑡)$ represents the instantaneous Hilbert phase of a given node 𝑛 at time 𝑡.

**Synchrony** 
- **mean** of $R(t)$ over time
- Degree of phase coupling between nodes in the network

**Metastability** 
- **standard deviation** of 𝑅(𝑡) over time
- Level of flexible switching between a state of synchrony and asynchrony.


## [[Criticality]]

In critical systems, the **size of population events will follow a power-law distribution**

In neural systems, such events have been related to **neuronal avalanches**, where the activation of one of the network elements triggers a response of other elements, until activity dies out.

>[!Note] Neuronal avalanches
>Size and duration of such neuronal avalanches follow a power-law distribution with exponent -1.5, at various levels, from local networks to large-scale activity.

**NEURAL AVALANCHES DETECTION**
- Method from ([[@shewNeuronalAvalanchesImply2009]]). 
- After time series from each excitatory node are Z-scored ($𝐸𝑖(𝑡) = 1 𝜎(𝐸𝑖 ) (𝐸𝑖 − 𝐸𝑖)$), we detect incursions beyond a threshold of ±2.3, thus identifying events that are distinct from noise with a probability of p<0.01. Then, we define events as the time points where the signal first crossed the threshold and avalanches as continuous periods of time where events occurred in the network.

**CRITICALITY MEASUREMENT**
- Method from [[@hellyerLocalInhibitoryPlasticity2016]]
- Comparing the distribution of avalanche sizes in neural data with a truncated power-law with exponent -1.5. Shortly, we computed the measure 𝑘 using:

![[Pasted image 20230220140046.png]]

where:
- 𝑚 = 10 is the number of logarithmically spaced points 𝛽𝑛 between the minimum and maximum avalanche sizes, 
- $𝐹^{𝑃𝐿}$ is the cumulative distribution of a -1.5 exponent power-law, truncated so that the maximum avalanche size is the number of nodes in our model (𝑁 = 78)
- $𝐹^{𝑁𝐴}$ is the cumulative distribution of avalanche sizes in the model data.

>[!warning]
> $k \approx 1$ means that the system is close to criticality
> $k < 1$ subcritical system
> $k > 1$ supercritical system

---
## References

[[@pascoadossantosMultiscaleEffectsExcitatoryInhibitory2022]]
[[@shewNeuronalAvalanchesImply2009]]
[[@hellyerLocalInhibitoryPlasticity2016]]