---
title: Low-Dimensional Spatiotemporal Dynamics Underlie Cortex-wide Neural Activity
authors: Camden J. MacDowell, Timothy J. Buschman
year: 2020
---

Cognition arises from the dynamic flow of neural activity through the brain. 

>[!Note] Keypoints
>
>To capture these dynamics, we used **mesoscale calcium imaging** to record neural activity across the *dorsal cortex of awake mice*.
>We found that the **large majority of variance in cortex-wide activity (75%) could be explained by a limited set of 14 ‘‘motifs’’** of neural activity. 
>- Each motif captured a unique spatiotemporal pattern of neural activity across the cortex. 
>- These motifs generalized across animals and were seen in multiple behavioral environments. Motif expression differed across behavioral states, and specific motifs were engaged by sensory processing, suggesting the motifs reflect core cortical computations. 

Together, our results show that cortex-wide neural activity is highly dynamic but that these **dynamics are restricted to a low-dimensional set of motifs**, potentially allowing for efficient control of behavior.

---

### INTRODUCTION

#### Previous work

>[!success] RESULTS
>**Associated** particular *computations* with *specific spatiotemporal patterns of neural activity* across the brain [1-3]
>
>*Sequential activation* of *primary sensory* and then *higher-order cortical regions* **underlies** perceptual decision making in both mice [4] and monkeys [5, 6].
>
>Specific *spatiotemporal patterns of cortical regions* are **engaged** during *goal-directed behaviors* [7], motor learning and planning [8, 9], evidence accumulation [10], and sensory processing [11]. 
>
>Has begun to **codify** these dynamics, either in the synchronous activation of brain regions [3, 12] or in the propagation of waves of neural activity within and across cortical regions [13, 14].

Together, this work suggests cortical activity is highly dynamic, evolving over both time and space, and that these dynamics play a computational role in cognition [15, 16].

>[!warning] Limitations
>**Restricted** to *specific regions* and/or *specific behavioral states*
>- Don't know how neural activity evolves across the entire cortex
>- Dynamics are similar across individuals?
>- How dynamics relate to behavior?

Difficulty of quantifying the spatiotemporal dynamics of neural activity across the brain


#### How are they adressing the problem?

**Mesoscale imaging** to *measure neural activity across the dorsal cortical surface* of the moues brain [17].

**Convolutional factorization approach** to *identify dynamic "motifs" of cortex-wide neural activity*.

>[!success] RESULTS
>Each motif **captured** a *unique spatiotemporal pattern of neural activity* as it evolved across the cortex.
> 
>Motifs **captured** the *dynamic flow of neural activity across regions*
> - Explained cortex-wide neural activity better than ‘‘functional connectivity’’ network measures.
> 
>Motifs **clustered** into a *limited set of 14 different spatiotemporal ‘‘basis’’ motifs* that were consistent across animals
>
>The basis motifs **captured** the *majority of the variance in neural activity* in different behavioral states and in multiple sensory and social environments. 
>
>Specific motifs were **selectively engaged** by *visual and tactile sensory processing*.
>- Suggesting the motifs may reflect core cortical computations.

Together, our results suggest cortex-wide neural activity is highly dynamic but that these dynamics are low-dimensional: they are constrained to a small set of possible spatiotemporal patterns.

---

### RESULTS

#### Discovery of Spatiotemporal Motifs of Cortical Activity in Awake, Head-Fixed Mice

We performed **widefield ‘‘mesoscale’’ calcium imaging** of the *dorsal cerebral cortex* of *awake*, *head-fixed mice* expressing the fluorescent calcium indicator GCaMP6f in cortical pyramidal neurons.

A **translucent-skull prep** provided *optical access to dorsal cortex*, allowing us to track the dynamic evolution of neural activity across multiple brain regions, including visual, somatosensory, retrosplenial, parietal, and motor cortex.

>[!Note] Imaging
> ![[Pasted image 20230320103624.png]]
> 
> *Red dot* denotes **bregma**. 
> 
> Cortical **parcellation** follows *Allen Brain Atlas*. 
> 
> General anatomical parcels are labeled. **Motor**, motor cortex; **SS**, somatosensory cortex; **Parietal**, parietal cortex; **RSP**, retrosplenial cortex; **Visual**, visual cortex
> 
> Nine mice were imaged for 12 min a day for 5–6 consecutive days.

Initially characterized the dynamics of ‘‘spontaneous’’ neural activity when mice were not performing a specific behavior. (N = 48 sessions across 9 mice, 5–6 sessions per mouse, each session lasted 12 min, yielding a total of 9.6 h of imaging)

These recordings revealed rich dynamics in the spatiotemporal patterns of neural activity across the cortex


#### Capture, quantify, and characterize the dynamic patterns of activity in an unbiased manner

We used *convolutional non-negative matrix factorization* (CNMF) to discover repeated spatiotemporal patterns of neural activity, in an unsupervised way.

CNMF identified motifs of neural activity; these are dynamic patterns of neural activity that extend over space and time.


#### Motifs Capture the Dynamic Flow of Neural Activity across the Cortex

Tested whether motifs simply reflected the coactivation of brain regions or if they captured the dynamic flow of neural activity between regions.










Do you know these papers: Spatiotemporal refinement of signal flow through association cortex during learning, Low-Dimensional Spatiotemporal Dynamics Underlie Cortex-wide Neural Activity, Spontaneous cortical activity alternates between motifs defined by regional axonal projections, Single-trial neural dynamics are dominated by richly varied movements, On The Biophysical Complexity of Brain Dynamics: An Outlook, Cortical signatures of wakeful somatosensory processing, Spontaneous behaviors drive multidimensional, brainwide activity?