Convolutional non-negative matrix factorization (CNMF)
- With a penalty term to facilitate discovery of repeating sequences

**Given image**                          -> _P x 1_ vector of pixel values.
**Recording image sequence** -> _P x T_ matrix, (_T_ num of time points in the recording).

This matrix can be **factorized** into:
**K smaller matrices**  -> _P_ x _L_  short sequences of events (e.g., motifs)
**W set of motifs**        -> _P_ x _K_ x _L_ tensor
L -> max duration of motifs
K -> max number of motifs

Each pattern is expressed over time according to:
**H temporal weighting matrix** -> _K_ x _T_ 

Original data matrix can be approximated:
Sum of K convolutions between the motifs in W and their corresponding temporal weightings in H

![[Pasted image 20230322150833.png]]

Spatiotemporal penalty term into the cost function of the multiplicative update algorithm. In brief, this reduces redundancy between motifs: 
1) multiple motifs do not describe the same sequence of activity; 
2) a single motif is not temporally split into separate motifs; and 
3) motifs are encouraged to be non-overlapping in time.





---

#### Activity computation

Normalized activity was computed as change in fluorescence, e.g., 

ΔF/F over time according to . Baseline fluorescence, F0, was computed as the rolling mean of a 9750ms window (130 time points) across the entire recording duration. ΔF/F was computed individually per pixel and using the baseline fluorescence for each time point

---

#### Hemodynamics cleaning

Two more sensors capturing 410nm 470nm light, compute diff between these two then substract from calcium activity.