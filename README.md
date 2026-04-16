# Deconvolution-Astrocyte

This repository contains the code and data supporting the study “Integrative Framework for Reference-Free Transcriptomic Deconvolution and Metabolic Profiling of Astrocytes across Alzheimer’s Disease Progression.” The project focuses on the integration of reference-free transcriptomic deconvolution methods with genome-scale metabolic modeling to characterize astrocyte-specific alterations along the continuum from mild cognitive impairment (MCI) to Alzheimer’s disease (AD).

In this work, bulk hippocampal transcriptomic data are used to infer astrocyte-associated gene expression profiles across four biological states: Control, Incipient MCI, Moderate MCI, and Severe MCI/Alzheimer’s disease. Two complementary deconvolution approaches, CDSeq and DECODER, are applied to disentangle cell-type-specific signals from heterogeneous transcriptomic data without the need for predefined reference signatures. This strategy enables the reconstruction of astrocyte-relevant transcriptional programs directly from bulk data.

The inferred astrocyte signatures are subsequently integrated into genome-scale metabolic models (GEMs) to generate condition-specific representations of astrocyte metabolism. These models are constrained using transcriptomic information and analyzed using flux-based approaches, allowing the identification of metabolic pathway alterations associated with disease progression. Through this framework, we aim to capture the progressive metabolic rewiring of astrocytes and identify key vulnerabilities linked to neurodegeneration.

To ensure biological relevance, an external validation strategy is implemented using independent single-nucleus RNA sequencing (snRNA-seq) data from astrocytes in the entorhinal cortex. Pseudobulk profiles are generated using a donor-aware approach and compared with deconvolution-derived signatures. This validation demonstrates that CDSeq-derived profiles achieve moderate but biologically meaningful concordance with single-cell reference data (r ≈ 0.43–0.44), alongside the preservation of canonical astrocyte markers such as GFAP, AQP4, and SLC1A2, as well as enrichment of astrocyte-associated pathways. These results indicate that the inferred signals capture biologically relevant astrocyte programs despite cross-platform and cross-region differences.

The analytical framework follows a systems biology approach in which transcriptomic data are first deconvolved to extract cell-type-associated signals and subsequently integrated into a generic astrocyte metabolic network. This enables the generation of context-specific models that can be analyzed to compare metabolic flux distributions across disease stages. The resulting outputs provide insight into pathway-level alterations, including dysregulation of lactate metabolism, the glutamine–glutamate cycle, and oxidative stress-related pathways.

The repository includes the processed transcriptomic datasets, deconvolution outputs, condition-specific metabolic models, and scripts required to reproduce the full analytical workflow, from data preprocessing to validation and metabolic simulation. The structure of the repository is organized to facilitate reproducibility and reuse, allowing users to follow the complete pipeline and adapt it to other datasets or cell types.

From a methodological perspective, this work highlights the importance of combining complementary computational approaches. CDSeq provides statistically robust and biologically coherent profiles through probabilistic modeling, whereas DECODER offers sensitivity to absolute transcriptional variation. The integration of both methods within a unified framework enables a more comprehensive characterization of astrocyte biology.

From a biological standpoint, the results reinforce the central role of astrocytes in maintaining brain metabolic homeostasis and demonstrate that their metabolic function is progressively disrupted during neurodegeneration. The observed changes suggest a transition from homeostatic to reactive and ultimately dysfunctional astrocyte states, contributing to the metabolic vulnerability associated with Alzheimer’s disease.

All data and scripts are made available to ensure transparency, reproducibility, and to support further methodological and biological exploration by the research community. This framework is designed to be extensible to other cell types, brain regions, and multi-omic datasets, providing a scalable platform for studying cell-type-specific metabolism in complex diseases.

For questions or potential collaborations, please contact:

Maria Andrea Angarita Rodríguez  
Doctoral Candidate in Biological Sciences  
MSc in Bioinformatics  
maria.angaritar@javeriana.edu.co  

Laura Rodríguez  
rodriguezmlauran@javeriana.edu.co  
Biologist
