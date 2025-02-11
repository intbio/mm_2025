# Workshop: Introduction to Rosetta

## Description
- We will outline basic methods of working with protein design using pyRosetta, ProteinMPNN and RFDiffusion. 
- Duration: 90 minutes
- Objectives: be able to 
    - Understand how to setup modeling with Rosetta 
    - Understand how to setup protein folding simulations in Rosetta
    - Understand how to vary a binding sequence using ProteinMPNN
    - Understand how to generate new protein scaffolds using RFDiffusion 

    


## Jupyter notebooks
- [PyRosetta Workshops](https://rosettacommons.github.io/PyRosetta.notebooks/).
- The github repo (PyRosetta) is [here](https://github.com/RosettaCommons/PyRosetta.notebooks)
- ProteinMPNN [basic](https://colab.research.google.com/github/sokrypton/ColabDesign/blob/v1.1.0/mpnn/examples/proteinmpnn_in_jax.ipynb) and [example](https://colab.research.google.com/github/dauparas/ProteinMPNN/blob/main/colab_notebooks/quickdemo.ipynb)
- [RFDiffusion](https://colab.research.google.com/github/sokrypton/ColabDesign/blob/v1.1.1/rf/examples/diffusion.ipynb#scrollTo=tVAE0BrnZoRR)
   


## Required software and resources
- Easiest way is to use Google Colab Google Drive - see tutorial for initialization instructions. However, this will require a lengthy download.
- Or you need local access to a Jupyter notebook evironment with pyRosetta installed, see [here](http://www.pyrosetta.org/dow)
- Or use SandBox cluster **rosetta** conda environment.

## Learning resources
- [pyRosetta tutorials](https://rosettacommons.github.io/PyRosetta.notebooks/)
- [Colab Design](https://github.com/sokrypton/ColabDesign)
- [RFDiffusion](https://github.com/RosettaCommons/RFdiffusion/blob/main/README.md#binder-design)


## Assignments

Take a structure of interest (with 2 or more protein chains):

1. Using pyRosetta, analyze energy between any two close residues of separate chains, output various energy terms.See 03.02-Analyzing-energy-between-residues.ipynb 
2. (со звуздочкой) Using pyRosetta, take an arbitrary sequence of 10 amino acids. Try to do folding. Explore different lowest conformations depeding on the number of Monte-Carlo steps. Visualize results. See 04.01-Basic-Folding-Algorithm.ipynb 
3. Use RFDiffusion to generate a new binder scaffold for the target protein. Use ProteinMPNN to generate the amino acid residues of the new binder. Use AlphaFold to check whether a complex similar to the original structure is formed. 

### Troubleshooting
- Consult with the seminar protocol/recording
- Ask questions in Slack
