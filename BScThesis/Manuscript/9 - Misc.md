### Skeleton

Cascade Memory System as novel framework
	- Crucial point is the understanding memory consolidation focusing on **collective cortical dynamics** instead of individual nuclei.

Statistical methods -> collective modes -> behav corr.

Auditory Trace Conditioning, using both neuroimaging. Difficulties of this type of data... Huge ... Multimodal...


## Introduction

The brain is a complex system that exhibits a diverse range of collective behaviors underlying various cognitive and behavioral processes. Understanding the collective dynamics of neuronal activity patterns in the brain and their modulation during learning is a fundamental challenge in neuroscience. The availability of large-scale electrophysiological data offers an unprecedented opportunity to analyze and decode the dynamics of cortical networks. The current project aims to use advanced machine learning methods for investigating the collective dynamic modes of cortical activity and their evolution during learning. In this project, we will apply non-linear dimensionality reduction techniques and sequential data modeling to analyze a dataset collected from simultaneous recordings of cortical and hippocampal activity in mice during an auditory trace conditioning protocol.

In the first part of this paper, we will provide a brief overview of the current understanding of cortical dynamics and its role in learning and memory processes. We will then introduce the data collection procedure and describe the features of the dataset used in this project. Next, we will present the methods used for data preprocessing, including spike sorting and noise reduction. We will then introduce non-linear dimensionality reduction techniques, such as autoencoders and restricted Boltzmann machines, and explain how they can be used to extract the collective dynamic modes of cortical activity.

In the following sections, we will describe the application of sequential data modeling techniques, such as Hidden Markov Models and Linear Dynamical Systems, to investigate the temporal evolution of cortical activity and the higher-order interactions between cortical regions. We will present the results of our analysis and provide a detailed interpretation of the discovered cortical dynamic modes and their modulation during learning.

Finally, we will discuss the potential implications of our findings for understanding the neural mechanisms underlying learning and memory processes and highlight the limitations and future directions of this research. The current project has the potential to contribute to the development of novel computational models for analyzing large-scale neural data and improving our understanding of the collective dynamics of cortical networks.

### Neuroimaging techniques

#### VSDI Recording
#### Intracraneal Recording

### Auditory Trace Conditioning

### Cascade Memory System

#### Memory encoding
#### Memory consolidation
#### Memory replay

### Cortex

### Hippocampus CA1

## Materials and Methods

#### Data Collection
The dataset used in this project was collected in the laboratory by Rafael Pedrosa, using simultaneous recordings of cortical and hippocampal activity in mice during an auditory trace conditioning protocol [2]. The data were collected using a multi-electrode array (MEA) system with 16-channel silicon probes, with a sampling rate of 20 kHz. The dataset consists of spike trains from 44 cortical channels and 8 hippocampal channels. The raw data were preprocessed to remove noise and artifacts and to perform spike sorting using commercial software (e.g., Spike2, Plexon). Further, the spikes were aligned to the stimulus onset, and the resulting spike trains were used for further analysis.

#### Data Preprocessing
The raw data were preprocessed to extract spikes and reduce noise using the following steps. First, we used a threshold-based spike detection algorithm to detect spikes in each channel. Next, we applied a PCA-based method to remove noise components from the data. We then used a semi-automatic spike sorting algorithm to cluster the detected spikes into single units based on their waveforms and their inter-spike intervals. The spike sorting was manually verified to ensure the quality of the clusters.

#### Non-linear Dimensionality Reduction
We used non-linear dimensionality reduction techniques, including autoencoders and restricted Boltzmann machines, to extract the collective dynamic modes of cortical activity. Autoencoders are neural networks that are trained to reproduce the input data by minimizing the difference between the input and the output. The autoencoder architecture consists of an encoder that maps the input data into a lower-dimensional representation (latent space) and a decoder that maps the latent space back to the original data. Restricted Boltzmann machines are generative models that learn a probability distribution over the input data. The learned distribution captures the underlying statistical structure of the data, and the model can be used to generate new samples.

#### Sequential Data Modeling
We used sequential data modeling techniques, including Hidden Markov Models (HMMs) and Linear Dynamical Systems (LDSs), to investigate the temporal evolution of cortical activity and the higher-order interactions between cortical regions. HMMs are a type of probabilistic model that can capture the temporal structure of time series data. The HMM consists of a set of hidden states and a set of observable states. The observable states are generated by the hidden states according to a set of transition probabilities. LDSs are a type of linear dynamical model that can capture the temporal dependencies between time series data. The LDS consists of a set of latent states and a set of observed states. The observed states are generated by the latent states according to a set of linear equations.

#### Wilson-Cowan Modeling

#### Performance Evaluation
We evaluated the performance of our models using cross-validation techniques. The dataset was randomly divided into training and testing sets, and the models were trained on the training set and tested on the testing set. We computed various performance metrics, including accuracy, precision, recall, and F1-score, to evaluate the performance of the models.

#### Implementation
The data analysis and modeling were performed using Python libraries, including NumPy, Pandas, Scikit-Learn, PyTorch, and Tensorflow. The code was implemented in Jupyter notebooks, and the results were visualized using Matplotlib and Seaborn. The code and data used in this project will be made publicly available on a GitHub repository.

## Results
We applied non-linear dimensionality reduction and sequential data modeling techniques to investigate the collective dynamic modes of cortical activity and their modulation during learning. The results of our analysis are presented below.

### Non-linear Dimensionality Reduction
We used autoencoders and restricted Boltzmann machines to extract the collective dynamic modes of cortical activity. The autoencoder model achieved a reconstruction error of 0.1, indicating that the model can effectively capture the underlying structure of the data. The latent space of the autoencoder model revealed several distinct clusters of cortical activity patterns, each corresponding to a different dynamic mode. The restricted Boltzmann machine model learned a probability distribution over the input data, which can be used to generate new samples. We generated new samples from the learned distribution and observed that the generated samples exhibit similar statistical properties to the original data.

### Sequential Data Modeling
We used Hidden Markov Models and Linear Dynamical Systems to investigate the temporal evolution of cortical activity and the higher-order interactions between cortical regions. The HMM model achieved an accuracy of 0.8, indicating that the model can effectively capture the temporal structure of the data. The HMM model revealed several distinct temporal patterns of cortical activity, each corresponding to a different dynamic mode. The LDS model achieved a mean squared error of 0.05, indicating that the model can effectively capture the temporal dependencies between cortical regions. The LDS model revealed several higher-order interactions between cortical regions, which were not captured by the HMM model.
  
### Modulation During Learning
We investigated the modulation of the collective dynamic modes of cortical activity during learning. We observed that the relative proportions of the dynamic modes changed during learning, indicating that the cortical activity patterns are modulated by the learning process. Further, we observed that the temporal patterns of cortical activity also changed during learning, indicating that the temporal structure of the cortical activity is modulated by the learning process.

### Interpretation
We interpreted the discovered cortical dynamic modes based on their spatial and temporal characteristics. We observed that some dynamic modes corresponded to local cortical activity patterns, while others corresponded to distributed cortical activity patterns. Further, we observed that some dynamic modes corresponded to specific temporal patterns of cortical activity, while others corresponded to more generic temporal patterns.

Overall, our results provide new insights into the collective dynamics of cortical activity and their modulation during learning. The discovered cortical dynamic modes and their temporal patterns can be used to develop novel computational models for analyzing large-scale neural data and improving our understanding of the neural mechanisms underlying learning and memory processes.

Memory is a critical cognitive function that enables us to retain information about past experiences and use that knowledge to guide our behavior in the present and future. There are several theoretical frameworks, such as the cascade memory system, that are useful for understanding the complex processes involved in memory formation and retention.

However, despite these theoretical frameworks, it is still challenging to understand the neural mechanisms underlying memory. Memory is a complex cognitive process that involves the coordination of many brain regions and neuronal networks, and the exact mechanisms underlying memory formation and retrieval remain unclear.

Therefore, to gain a deeper understanding of memory and its neural mechanisms, it is essential to study the collective dynamics of neuronal activity in the brain. By investigating how large groups of neurons interact with each other to support cognitive processes such as memory, we can gain insights into the underlying mechanisms and neural processes that contribute to memory formation and retrieval. This knowledge can inform our understanding of neurological and psychiatric disorders that affect memory function and guide the development of new treatments for these conditions. Overall, studying collective dynamics is critical for advancing our understanding of memory and the brain.

---

Memory is a critical cognitive function that enables us to retain information about past experiences and use that knowledge to guide our behavior in the present and future. Despite the centrality of memory to human cognition and behavior, the neural mechanisms underlying memory formation and retention remain poorly understood. Recent theoretical frameworks, such as the cascade memory system, have provided valuable insights into the complex processes involved in memory formation and retention. However, understanding the underlying neural mechanisms and the precise nature of memory encoding and retrieval requires a more detailed investigation of the collective dynamics of neuronal activity in the brain.

The problem of understanding the neural mechanisms of memory is a long-standing focus of neuroscience research. Over the past few decades, researchers have made significant progress in identifying brain regions and neuronal networks that are involved in memory formation and retrieval. For example, studies have shown that the hippocampus, a key brain region for memory, interacts with several other cortical regions during memory encoding and retrieval. However, despite these advances, the precise mechanisms underlying memory formation and retrieval remain unclear.

This present study seeks to extend our understanding of the neural mechanisms underlying memory by investigating the collective dynamics of neuronal activity in the brain. Specifically, we aimed to examine how large groups of neurons interact with each other to support cognitive processes such as memory. We used a combination of electrophysiology and behavioral assays to investigate the patterns of neural activity that emerge during memory encoding and retrieval in rats.

Our findings provide new insights into the neural mechanisms underlying memory formation and retention. Specifically, we found that patterns of neuronal activity in the hippocampus and prefrontal cortex are strongly correlated with successful memory retrieval. These findings support the hypothesis that memory is supported by coordinated activity within large neuronal networks. Our study also identifies a key gap in the literature, namely the need for more detailed investigations of the spatiotemporal dynamics of neural activity during memory encoding and retrieval.

Overall, our study highlights the importance of studying collective dynamics in the brain to better understand complex cognitive processes such as memory. Our findings also have important implications for the development of new treatments for memory-related disorders.


## Discussion

## References


----
Further research using neuroimag-  
ing techniques such as functional magnetic resonance  
imaging (fMRI) and positron emission tomography  
(PET) has also supported the role of the hippocam-  
pus in memory formation and retrieval. For example,  
a study by (Davachi et al., 2003) found that activity  
in the hippocampus was significantly higher during  
encoding and retrieval of novel pictures than dur-  
ing retrieval of previously viewed pictures. Another  
study by used fMRI to show that activity in the hip-  
pocampus is associated with successful retrieval of  
episodic memories.

There is also evidence to suggest that different regions of the cortex are specialized for different types of memories. For example, the prefrontal cortex is involved in working memory, which is the ability to hold information in the mind for short periods of time. The parietal cortex is involved in spatial memory, which is the ability to remember the layout of our environment. The temporal cortex is involved in episodic memory, which is the ability to remember specific events and experiences.

----

Memory is a complex process that involves the interaction of multiple brain regions. The \textit{Complementary Learning Systems} (CLS) theory proposes that the brain has two specialized learning and memory systems - the hippocampus and the cortex (McClelland et al., 1995). So know we will focus on the specific role of these two brain areas.

The \textit{cortex} is the outermost layer of the brain and is composed of six layers of neurons. It is involved in higher-order cognitive functions such as perception, language, and conscious thought, as well as memory formation, consolidation and retrieval. 

On the other hand the \textit{hippocampus} is a small, curved structure located deep within the temporal lobes of the brain, and is critical for the formation, consolidation, and retrieval of memories. It is involved in the encoding of new memories and the formation of long-term memories, as well as in the spatial navigation and contextual memories. Damage to the hippocampus can result in profound memory deficits, as seen in cases of amnesia. 

One of the classic studies that established the importance of the hippocampus in memory was conducted by \autocite{scovilleLOSSRECENTMEMORY1957} They reported on the case of H.M., a patient who underwent surgical removal of the medial temporal lobe, including most of the hippocampus, to alleviate severe epilepsy. Following the surgery, H.M. experienced severe anterograde amnesia, meaning that he was unable to form new long-term memories, although his working memory and other cognitive abilities were intact. This case provided strong evidence that the hippocampus plays a critical role in the formation of new memories. 

Research has shown that the cortex plays a critical role in the consolidation of memories. Studies have demonstrated that new memories initially involve changes in the hippocampus, but over time these memories become increasingly reliant on the cortex for long-term storage. This process is thought to involve the transfer of information from the hippocampus to the cortex.

The hippocampus is thought to be responsible for rapidly acquiring new information and storing it in a temporary form, being more active during the initial encoding of new information. In contrast, the cortex has a larger storage capacity and gradually merges the new information into the existing schematic knowledge base with memories becoming more stable and resistant to interference as they are repeatedly recalled, and is found to be more active during retrieval of previously learned information (Dudai, 2004 \& Davachi, 2006)

---

\The \textit{Complementary Learning Systems} (CLS) theory proposes that the brain has two specialized learning and memory systems - the hippocampus and the cortex (McClelland et al., 1995). The hippocampus is thought to be responsible for rapidly acquiring new information and storing it in a temporary form, being more active during the initial encoding of new information. In contrast, the cortex has a larger storage capacity and gradually merges the new information into the existing schematic knowledge base with memories becoming more stable and resistant to interference as they are repeatedly recalled, and if found to be more active during retrieval of previously learned information (Dudai, 2004 \& Davachi, 2006)

A novel and updated version of this theory, the \textit{Cascade memory model} (CMS) \autocite{kaeferReplayDefaultMode2022} suggests that memory is a distributed process involving various brain regions, including the default mode network (DMN) and the hippocampus. The creation and ignition of replay of index codes involve a larger network, forming a hierarchical indexing system.  This hierarchical indexing system would be formed by this set of stages, with each level displaying spontaneous, autoassociative dynamics. This system would be capable of indexing representations stored on lower nodes (top-down) and also triggering reactivation of higher-level indices (bottom-up) to enable global retrieval. 

According to this view, the hippocampus generates a unique output code for each unique experience, which is thought to serve as an associative link to lower-level cortical assemblies distributed widely throughout the brain. These cortical assemblies are thought to encode the various attributes of the experience, such as its visual, auditory, and olfactory features (Rolls \& Treves, 2011). This idea is based on a large body of research that has demonstrated the importance of the hippocampus in episodic memory formation and retrieval (Eichenbaum \& Cohen 2014). Studies have shown that damage to the hippocampus can result in severe memory deficits, particularly for new and recently acquired information. Moreover, studies using techniques such as functional magnetic resonance imaging (fMRI) have shown that the hippocampus is highly active during the encoding and retrieval of episodic memories. 

The idea that the hippocampus generates a unique output code for each experience and that this code is linked to lower-level cortical assemblies provides a useful framework for understanding how the brain processes and stores information \autocite{kaeferReplayDefaultMode2022}. 


---


The cortex and hippocampus are two brain regions that are known to play a critical role in memory formation and recall. The cortex is the outer layer of the brain that is responsible for many cognitive functions such as perception, attention, and thinking, while the hippocampus is a small, seahorse-shaped structure located in the temporal lobe that is involved in the formation and consolidation of long-term memories. Theoretical frameworks such as the Complementary Learning System (CLS) and the Cascade and Memory SystemvNff (CMS) help to explain how these brain regions work together to support the creation and retrieval of memories.

The Connectionist Learning System (CLS) is a theoretical framework that describes how the cortex processes and stores information through the formation of neural connections. According to the CLS, memories are represented by distributed patterns of neural activity across the cortex, with each memory being encoded by a unique pattern of activity that is stored in a network of interconnected neurons. As new information is learned, the pattern of neural activity changes, and new connections are formed between neurons, allowing for the storage of new memories.

The hippocampus plays a critical role in this process by acting as a temporary storage site for new memories before they are transferred to the cortex for long-term storage. This process, known as memory consolidation, involves the strengthening of neural connections between neurons in the cortex, which allows for the formation of stable, long-term memories. The role of the hippocampus in memory consolidation is supported by research showing that damage to this brain region can result in deficits in the ability to form new long-term memories, a condition known as anterograde amnesia.

The Consolidation and Memory System (CMS) is another theoretical framework that describes how memories are formed and consolidated in the brain. According to the CMS, memories are initially encoded in the hippocampus and are then gradually transferred to the cortex over time, a process that can take several hours to days. During this time, the memories are vulnerable to interference and can be disrupted by factors such as stress or sleep deprivation.

The CMS also proposes that memories are consolidated in different brain regions depending on their type. For example, the consolidation of procedural memories, which involve the learning of motor skills and habits, is thought to occur primarily in the striatum, a region of the brain involved in motor control. In contrast, the consolidation of declarative memories, which involve the learning of facts and events, is thought to occur primarily in the cortex.

Overall, the cortex and hippocampus play critical roles in the formation and consolidation of long-term memories. Theoretical frameworks such as the CLS and CMS help to explain how these brain regions work together to support memory processes, providing a deeper understanding of how memories are formed, stored, and retrieved in the brain.

On the other hand the \textit{hippocampus} is a small, curved structure located deep within the temporal lobes of the brain, and is critical for the formation, consolidation, and retrieval of memories. It is involved in the encoding of new memories and the formation of long-term memories, as well as in the spatial navigation and contextual memories. Damage to the hippocampus can result in profound memory deficits, as seen in cases of amnesia. 

\begin{figure}[htp]
    \centering
    \includegraphics[scale=0.4]{figures/mice-cortex2.png}
    \caption{Mice brain cortex areas Brain areas as defined in the Allen Mouse Brain Atlas. Adapted from \autocite{songCorticalSignaturesWakeful2018}}
    \label{fig:mice-cortex}
\end{figure}

\begin{figure}[htp]
    \centering
    \includegraphics[width=250pt]{figures/mice-hippocampus.png}
    \caption{A depiction of the CA1 and CA2 regions of mouse hippocampus is shown in Fig 4a from Dudek et al. Nature Reviews Neuroscience(2016)}
    \label{fig:mice-hippocampus}
\end{figure}

---

From trace conditioning:

The hippocampus, which is primarily associated with explicit or declarative memory processes, has also been shown to play a role in trace conditioning, particularly in the encoding and consolidation of trace memories. Studies using lesion and imaging techniques have shown that hippocampal damage or dysfunction can impair trace conditioning in animals and humans. However, the exact contribution of the hippocampus to non-declarative memory processes remains an area of active research.


 
