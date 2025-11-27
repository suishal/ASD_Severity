# Dissecting Gut Microbiome Variations in Autism Spectrum Disorder Clinical Symptoms and Severity  

## Overview

Autism spectrum disorder (ASD) is a heterogeneous neurodevelopmental condition with individualised needs. Although evidence implicates the role of gut microbiome in ASD pathophysiology, prior studies have overlooked its clinical heterogeneity, leaving unclear whether microbial variations contribute to clinical severity and specific symptoms. Here, we performed shotgun metagenomic sequencing on stool samples from 720 children with ASD (median age 8 years, 87% male) and 151 matched children without ASD. Children with ASD were stratified into three severity groups based on 14 symptom subscales covering core ASD symptoms and co-occurring psychopathologies. Both overall severity and individual symptoms were significantly associated with gut microbiome composition (R2 = 0.0017 - 0.0065, p < 0.05). Children with more severe ASD exhibited enrichment of opportunistic pathogens, such as Citrobacter freundii and Enterococcus faecalis, and depleted anti-inflammatory Pseudoflavonifractor capillosus and GABA synthesis. Symptom-specific analyses revealed that sensory atypicalities had the largest number of associated microbial markers and specifically linked to excess excitatory neurotransmitters (q < 0.2). These findings demonstrate that gut microbiome composition varies across the ASD severity spectrum. Imbalance in microbial excitatory/inhibitory neurotransmitter metabolism emerges as a plausible mechanism underlying sensory atypicalities. Such insights may inform the development of targeted microbial therapeutics for ASD. 

## Code Overview

The analytical pipeline includes:

- Unsupervised clustering (K-means) to identify ASD subtypes
- Dimensionality reduction and visualization (PCA)
- Batch effect correction
- Microbiome data preprocessing
- Taxonomic, pathway, and functional module analysis

## Dependencies

### R Packages
- `MMUPHin = 1.23.0`
- `Maaslin2 = 1.23.0`
- `vegan = 2.7.2`
- `ggplot2 = 4.0.1`
- `dplyr = 1.1.4`
- `MicrobiotaProcess = 1.22.0`

> Install MaAsLin2 from Bioconductor:
> ```r
> if (!require("BiocManager", quietly = TRUE))
>     install.packages("BiocManager")
> BiocManager::install("Maaslin2")
> ```

### Python (for `Kmeans.ipynb`)
- `numpy = 1.26.4`
- `pandas = 2.0.3`
- `scikit-learn = 1.5.1`
- `matplotlib = 3.7.2`
- `seaborn = 0.13.2`
