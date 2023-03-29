There are several neuroimaging techniques, which allow us to capture brain activity in order to study brain structure, function, and connectivity. Each technique has its own set of advantages and limitations. Here, we'll discuss some of the most commonly used techniques, and the ones that were used for the data collection of the mice brain activity we will analyze in this study.

Some of the most commonly used techniques include functional magnetic resonance imaging (fMRI), electroencephalography (EEG), magnetoencephalography (MEG), and positron emission tomography (PET).

Functional magnetic resonance imaging (fMRI) measures brain activity by detecting changes in blood flow associated with neural activity (Logothetis \& Wandell, 2004). It provides high spatial resolution, allowing researchers to visualize specific brain regions and networks involved in cognitive processes. However, it has limited temporal resolution and is susceptible to artifacts and signal distortion (Buxton, 2013). Additionally, fMRI is expensive and requires specialized equipment (Poldrack et al., 2011).

Electroencephalography (EEG) records electrical activity generated by the brain's neurons using electrodes placed on the scalp (Nunez \& Srinivasan, 2006). It provides high temporal resolution, making it ideal for studying the dynamics of neural activity (Buzsáki et al., 2012). EEG is portable and relatively inexpensive, but it has limited spatial resolution and is susceptible to artifacts from non-brain sources (Goncharova et al., 2003). Careful electrode placement and data preprocessing are necessary for accurate results (Cohen, 2014).

Magnetoencephalography (MEG) measures the magnetic fields generated by neural activity using highly sensitive sensors (Hämäläinen et al., 1993). Like EEG, MEG provides high temporal resolution and can capture the dynamics of brain activity (Baillet, 2017). MEG is less affected by artifacts compared to EEG (Hillebrand \& Barnes, 2002) and can localize sources of neural activity with reasonable accuracy (Hari \& Salmelin, 2012). However, MEG has limited spatial resolution compared to fMRI, is expensive, and requires specialized equipment (Baillet, 2017; Hari \& Salmelin, 2012).

Positron emission tomography (PET) is an imaging technique that uses radioactive tracers to measure brain metabolism and blood flow, providing insights into brain function (Phelps, 2000). PET can be used to study various aspects of brain function, such as neurotransmitter systems (Krause et al., 2000). However, PET is invasive due to the use of radioactive tracers and has lower spatial and temporal resolution compared to fMRI and EEG/MEG, respectively (Phelps, 2000; Rabiner \& Gunn, 2014).


---

Cortex-wide activity is classically studied with imaging techniques that rely on indirect correlates of neural activity, such as the blood-oxygen-level-dependent (BOLD) or intracellular calcium signals, whereas most of our knowledge of the hippocampus comes from microelectrode recordings [6,11]. While classical imaging methods allow for excellent spatial coverage, they suffer from limited spatial resolution. Microelectrode techniques, on the other hand, provide recordings with excellent temporal resolution but limited spatial information [12]. In particular, conventional widefield imaging using genetically encoded calcium indicators (GECIs) presents a significant temporal discrepancy in activity when compared with electrophysiology, due to the distinct nature of the recorded signals [13,14]. Cortical widefield voltage imaging using genetically encoded voltage indicators (GEVIs) in head-fixed mice provides a large-scale view on cortical activity with both high spatial and high temporal resolution, and it can be combined with electrode-based electrophysiology [15]. Here we describe the combination of cortical voltage imaging with hippocampal electrode recordings to simultaneously monitor activity both from the cortex and the hippocampus during rest and traditional behavioral tasks.

---
1. Algorithmic approach: While PCA, ICA, and GLM have proven to be useful in our current analysis, we aim to expand our methodological toolkit by incorporating more advanced machine learning techniques. This will allow us to identify and understand more complex patterns and relationships within the data. For instance, deep learning algorithms and non-linear dimensionality reduction methods, such as t-SNE (t-distributed Stochastic Neighbor Embedding) and UMAP (Uniform Manifold Approximation and Projection), could provide a deeper understanding of the data set structure and reveal additional insights into the underlying neural processes.

---

There are several neuroimaging techniques, which allow us to capture brain activity in order to study brain structure, function, and connectivity. Each technique has its own set of advantages and limitations. Here, we'll discuss some of the most commonly used techniques, and the ones that were used for the data collection of the mice brain activity we will analyze in this study.

\textit{Voltage-sensitive dye imaging (VSDI)} is a neuroimaging technique that uses a voltage-sensitive dye to visualize changes in membrane potential of large populations of neurons simultaneously. The dye is applied to the surface of the brain and excited with light of a specific wavelength, causing it to fluoresce. As neurons fire action potentials, there is a change in the electrical potential across their membranes, which alters the fluorescence of the dye. This change in fluorescence can be detected and used to create a map of neuronal activity across the brain surface. 

VSDI Neuroimaging of Whole-Cortex Novel techniques such as voltage-sensitive dye imaging (VSDI) have been developed to overcome these limitations.  VSDI allows researchers to visualize changes in neural activity in real-time with high spatial and temporal resolution.

Widefield voltage imaging serves as a valuable method for monitoring several cortical regions at once in conscious, active animals. In contrast to other proxies of brain activity, like calcium and glutamate indicators, voltage activity offers superior temporal resolution, akin to electrophysiology. \autocite{pedrosaCombiningCorticalVoltage2022}.

\textit{Intracraneal recording of Hippocampus CA1}: Intracranial recordings (ICR) are neuroimaging techniques used to record electrical activity directly from the brain using electrodes implanted within the brain tissue. These recordings provide high spatial and temporal resolution, making them a powerful tool for investigating brain function and understanding the mechanisms underlying neurological and psychiatric disorders.

However, intracranial recordings are invasive and can be associated with significant risks, so for human use are typically reserved for patients with severe neurological or psychiatric disorders who have not responded to other treatments.

---

\begin{figure}[htp]
    \centering
    \includegraphics[width=250pt]{figures/hemocleaning.png}
    \caption{Fingerprints of components before and after hemodynamic noise correction}
    \label{fig:hemodynamics}
\end{figure}

\begin{figure}[htp]
    \centering
    \includegraphics[width=250pt]{figures/cortex-avalanche.png}
    \caption{Collective cortex-wide activity. \textit{From \autocite{kaeferReplayDefaultMode2022}}}
    \label{fig:my_label}
\end{figure}

\textit{Independent component analysis} (ICA) is a statistical technique used to decompose a multivariate signal into independent, non-Gaussian components. ICA assumes that the observed signals are linear combinations of independent source signals, and it aims to recover the original sources from the mixed signals by estimating the mixing matrix.

ICA is commonly used in signal processing and data analysis to identify hidden structures and relationships in complex data, particularly in the context of blind source separation. For example, ICA has been used in neuroscience to separate the electrical signals measured from the scalp into independent components representing different brain sources. In finance, ICA has been used to identify patterns of market activity that are independent of each other.

Unlike PCA, which identifies the principal components that capture the most variation in the data, ICA aims to find the components that are statistically independent and non-Gaussian. This can be particularly useful when the sources are non-linearly mixed or when there are multiple sources contributing to the observed signals.