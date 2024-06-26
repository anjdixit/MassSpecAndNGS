# MassSpecAnalysis

This repo contains scripts which process Mass Spec and NGS data for DEL decoding, analysis, and yield determination. Scripts are written such that they are directly compatible with a Google Colab environment and will source files from any individual's Drive account.

1. LC MS Analysis and plots: Script to pair files exported from a ThermoFisher LC/MS (.txt with chromatogram data, .raw and .mzmL containing compressed spectra) and plot chromatograms, as well as associated spectra from a tunable peak picking function. Peak AUC and relative AUCs are also calculated.
2. NGS analysis and decoding: Script used to process fastq data obtained from NGS sequencing of hit compounds from DEL screens. Output files with analysis relating to sequence counts, building block decoding, UMI analysis, and compounds' replicate class are produced within the workflow and can be studied both within or outside the code to make decisions about further processing steps
3. SingleBeadAnalysis: Script to match individually barcoded wells containing single DEL beads and decode the expected compound and molecular weight for yield determination via truncate and full product identification using mass matching via MALDI-TOF.
