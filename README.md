# HyperBrain

This repository is the official implementation of "HyperBrain: Anomaly Detection for Temporal Hypergraph Brain Networks".

## Authors
[Sadaf Sadeghian](https://www.linkedin.com/in/sadaf-sadeghian-53b8b4174/), [Xiaoxiao Li](https://xxlya.github.io), [Margo Seltzer](https://www.seltzer.com/margo/)

### Abstract
Identifying unusual brain activity is a crucial task in neuroscience research, as it aids in the early detection of brain disorders. It is common to represent brain networks as graphs, and researchers have developed various graph-based machine learning methods for analyzing them. However, the majority of existing graph learning tools for the brain face a combination of the following three key limitations. First, they focus only on pairwise correlations between regions of the brain, limiting their ability to capture synchronized activity among larger groups of regions. Second, they model the brain network as a static network, overlooking the temporal changes in the brain. Third, most are designed only for classifying brain networks as healthy or disordered, lacking the ability to identify abnormal brain activity patterns linked to biomarkers associated with disorders. To address these issues, we present HyperBrain, an unsupervised anomaly detection framework for temporal hypergraph brain networks. HyperBrain models fMRI time series data as temporal hypergraphs capturing dynamic higher-order interactions. It then uses a novel customized temporal walk (BrainWalk) and neural encodings to detect abnormal co-activations among brain regions. We evaluate the performance of HyperBrain in both synthetic and real-world settings for Autism Spectrum Disorder and Attention Deficit Hyperactivity Disorder(ADHD). HyperBrain outperforms all other baselines on detecting abnormal co-activations in brain networks. Furthermore, results obtained from HyperBrain are consistent with clinical research on these brain disorders. Our findings suggest that learning temporal and higher-order connections in the brain provides a promising approach to uncover intricate connectivity patterns in brain networks, offering improved diagnosis.

## Requirements
* `python >= 3.7`, `PyTorch >= 1.4`, please refer to their official websites for installation details.
* Other dependencies:
```{bash}
pandas==0.24.2
tqdm==4.41.1
numpy==1.16.4
scikit_learn==0.22.1
numba==0.51.2
```

## Acknowledgement
We have utilized the code from [here](https://github.com/ubc-systopia/CATWalk) as the foundation of our implementation, customizing it extensively to align with our specific needs. Thanks to the authors for sharing their code.

