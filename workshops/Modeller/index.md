# Workshop: Protein structure modeling in Modeller, CollabFold, SwissModel

## Description
- We will obtain protein structure based on templates
- Duration: 60 minutes
- Objectives: be able to 
    - Prepare protein sequences for Modeller
    - Select a template based on sequence identity comparison
    - Align target sequence with the template
    - Model building
    - Model evaluation
    - CollabFold usage
    - Swiss-Model usage

## Jupyter notebook
- [modeller.ipynb](modeller.ipynb)

## AlphaFold2  
- [Collab notebook](https://colab.research.google.com/github/deepmind/alphafold/blob/main/notebooks/AlphaFold.ipynb)
- [CollabFold paper](https://www.biorxiv.org/content/10.1101/2021.08.15.456425v2)
- [ChimeraX example](https://www.youtube.com/watch?v=le7NatFo8vI&ab_channel=UCSFChimeraX)

## Swiss-Model  
- [Web server](https://swissmodel.expasy.org/)

## Required software and resources
- Access to a Jupyter notebook evironment with Python 3, modeller, MDanalysis, nglview, Bio libraries 
- Access to Google collab with GPUs
- To install modeller run in your conda environment "conda install -c salilab modeller", use license key "MODELIRANJE"

## Learning resources
- [Modeller tutorial](https://salilab.org/modeller/tutorial/)
- [Swiss-Model tutorial](https://swissmodel.expasy.org/docs/examples)
- [DOPE (Discrete Optimized Protein Energy) method](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2242414/pdf/2507.pdf)

## Assignments
Select YOUR PROTEIN sequence for modeling structure
1. Find protein of your interest, [BLAST](https://blast.ncbi.nlm.nih.gov/Blast.cgi?PROGRAM=blastp&PAGE_TYPE=BlastSearch&LINK_LOC=blasthome) it with "NON-REDUNDANT PROTEIN SEQUENCES" database and choose a sequence with 60% identity or less.
2. BLAST the chosen sequence with "PROTEIN DATA BANK PROTEINS" database to check if it contains the 3D structure for your sequence (it must NOT have 3D structure in PDB).

AlphaFold2 
1. Predict 3D structure of YOUR PROTEIN (choose small one or fragment); use one of ChimeraX or Collab. Add sequence coverage plot and structure image.  

Swiss-Model
1. Predict 3D structure of YOUR PROTEIN. Compare with AlphaFold2 structure. Do NOT use AlphaFold structures as a template, only experimental ones!

Modeller (based on tutorial)
1. Build model for any protein of your interest based on a single template. Perfom loop refine by LoopModel and DopeLoopModel if possible.

### Troubleshooting
- Consult with the seminar protocol/recording
- Ask questions in Telegram
