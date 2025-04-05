# Workshop: Protein structure modeling AlphaFold 2 / AlphaFold 3

## Description
- We will obtain protein structure based on templates
- Duration: 60 minutes
- Objectives: be able to
    - Prepare molecular sequences & PTMs for input
    - Select optimal launch parameters
    - Understand and interpret output metrics
    - Evaluate results of the prediction
    - Compare and cross-validate predicted structure models

## AlphaFold2  
- [Colab notebook](https://colab.research.google.com/github/sokrypton/ColabFold/blob/main/AlphaFold2.ipynb)
- [ColabFold paper](https://www.biorxiv.org/content/10.1101/2021.08.15.456425v2)
- [LocalColabFold](https://github.com/YoshitakaMo/localcolabfold)
- [ChimeraX example](https://www.youtube.com/watch?v=le7NatFo8vI&ab_channel=UCSFChimeraX)

## AlphaFold 3
- [Web server](https://alphafoldserver.com/)
- [Open-sourced model](https://github.com/google-deepmind/alphafold3)

## Required software and resources
- Access to a Jupyter notebook evironment with Python 3, MDanalysis, nglview, Bio libraries
- Access to PyMOL/ChimeraX
- Access to Google collab with GPUs

## Learning resources
- [AlphaFold 2 tutorial]()
- [AlphaFold 3 guide](https://swissmodel.expasy.org/docs/examples)

## Assignments
### 1. Select YOUR PROTEIN sequence for modeling structure
- Find protein of your interest, [BLAST](https://blast.ncbi.nlm.nih.gov/Blast.cgi?PROGRAM=blastp&PAGE_TYPE=BlastSearch&LINK_LOC=blasthome) it with "NON-REDUNDANT PROTEIN SEQUENCES" database and choose a sequence with 60% identity or less.
- BLAST the chosen sequence with "PROTEIN DATA BANK PROTEINS" database to check if it contains the 3D structure for your sequence (it must NOT have 3D structure in PDB).
- Check which PTMs can be introduced to the protein of your choice (e.g. check potential phosphorylation sites that can be predicted [NetPhos](https://services.healthtech.dtu.dk/services/NetPhos-3.1/)).
- If the protein is >700 amino acids, select a functionally important domain (e.g., based on UniProt annotations).

### 2. Structure Prediction with AlphaFold 2
   
Run two prediction modes:
- Standard mode (with MSA and templates, if available).
- Template-free and MSA free mode.

Note that each prediction will produce 5 models (rank 1 to 5 in the filename)

For each of two predictions do the following:
- Calculate pairwise RMSD between all 5 ranks produced (using the software of your choice, can be PyMOL, VMD, Python script with Bio.PDB, etc.).
- Record the maximum RMSD
- If max RMSD > 5 Å, identify regions with the highest structural divergence (use pLDDT and PAE from AlphaFold’s output).

Choose the best rank model from each of two predictions and compare pLDDT between them: Are there regions where prediction quality decreased without templates and MSA?

### 3. PTMs modeling with AlphaFold 3

Select 1-2 potential phosphorylation sites (or other PTMs) for your protein (e.g., predicted by [NetPhos](https://services.healthtech.dtu.dk/services/NetPhos-3.1/)).

Run AlphaFold 3 (AF3) prediction in two modes:
- Default
- Specifying residues with PTMs

Compare phosphorylated vs. native protein structures:
- Are there changes in secondary/tertiary structure?
- Are there new/lost interactions with other domains?
- Check pLDDT near modified residues: Did prediction confidence decrease?

### Troubleshooting
- Consult with the seminar protocol/recording
- Ask questions in Telegram
