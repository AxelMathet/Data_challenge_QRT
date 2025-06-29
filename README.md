# Data_challenge_QRT

This repository contains my submission for a data science competition organized by 'École Normale Supérieure' and 'College de France', in collaboration with the company QRT. The goal is to estimate the risk of death of patients based on their clinical and genetic data.
The full details are available at the following link: https://challengedata.ens.fr/participants/challenges/162/

### Dataset Description

Clinical Data (1 row per patient)
- ID: Unique patient identifier
- CENTER: Clinical center
- BM_BLAST: Bone marrow blast percentage
- WBC, ANC, MONOCYTES, HB, PLT: Various blood metrics
- CYTOGENETICS: Chromosomal abnormalities (e.g., 46,XX, monosomy 7)
- Molecular Data (1 row per somatic mutation per patient)


Molecular Data (1 row per patient's mutation)
- ID: Patient ID
- CHR, START, END: Genomic location
- REF, ALT: Reference and alternate nucleotides
- GENE, PROTEIN_CHANGE, EFFECT: Mutation details
- VAF: Variant Allele Frequency

Target Variables
- OS_YEARS: Overall survival time (in years)
- OS_STATUS: 1 if patient is deceased, 0 if still alive at last follow-up

Prediction
- ID: patient ID
- risk_score: predicted risk of death
