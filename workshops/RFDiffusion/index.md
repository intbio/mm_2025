# Workshop: Introduction to ProteinMPNN and RFDiffusion

## Description
- We will outline basic methods of working with protein design using ProteinMPNN and RFDiffusion. 
- Duration: 90 minutes
- Objectives: be able to 
    - Understand how to setup modeling with ProteinMPNN and RFDiffusion
    - Understand how to vary a binding sequence using ProteinMPNN
    - Understand how to generate new protein scaffolds using RFDiffusion 

## Jupyter notebooks
- [Workshop notebook](https://colab.research.google.com/drive/1aR63ETRxMPeEmmQtZKut65qAiF7LSy9A?usp=sharing)
- ProteinMPNN colabs [basic](https://colab.research.google.com/github/sokrypton/ColabDesign/blob/v1.1.0/mpnn/examples/proteinmpnn_in_jax.ipynb) and [example](https://colab.research.google.com/github/dauparas/ProteinMPNN/blob/main/colab_notebooks/quickdemo.ipynb)
- [ProteinMPNN Github](https://github.com/dauparas/ProteinMPNN)
- [RFDiffusion Colab](https://colab.research.google.com/github/sokrypton/ColabDesign/blob/v1.1.1/rf/examples/diffusion.ipynb#scrollTo=tVAE0BrnZoRR)
- [RFDiffusion Github](https://github.com/RosettaCommons/RFdiffusion/tree/main)

## Required software and resources
- Plenty of Google Colab notebooks to go around
- Local installation of RFDiffusion requires pyRosetta license: see the original repository for the details

## Learning resources
- [Colab Design](https://github.com/sokrypton/ColabDesign)
- [RFDiffusion](https://github.com/RosettaCommons/RFdiffusion/blob/main/README.md#binder-design)

## Assignments

Take a structure of interest with 2 (or more) interacting proteins:

1. Generate several dozen new sequences for the binding interface for one of the proteins (the rest of amino acids should remain untouched).
   - Calculate sequence recovery for the binding interface. How often does ProteinMPNN reproduce native residues of the interface?
   - Based on ProteinMPNN score, select a few sequences and use AlphaFold to check whether a complex with updated sequence is similar to the original structure. 
2. Use RFDiffusion to generate a new binder scaffold for the target protein. Use ProteinMPNN to generate the amino acid residues of the new binder. Use AlphaFold to check whether a complex similar to the original structure is formed. 

### Troubleshooting
- Consult with the seminar protocol/recording
- Ask questions in Telegram
