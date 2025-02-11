# Workshop: Using PLUMED to enhance sampling in Gromacs

## Description
- We will outline basic methods of working with PLUMED.
- Duration: 90 minutes
- Objectives: be able to 
    - Setup simulations using PLUEMD+GROMACS
    - Define collective variables
    - Setup various types of biased simulations
    - Perform steered MD
    - Perform Metadynamics simulations
    


## Jupyter notebooks
- We follow [this tutorial](https://github.com/intbio/MolModEdu/tree/master/PLUMED) but use updated files.
- [plumed_intro.ipynb](plumed_intro.ipynb)
- [plumed_bias.ipynb](plumed_bias.ipynb)
- [plumed_metad_intro.ipynb](plumed_metad_intro.ipynb)



## Required software and resources
- Access to a Jupyter notebook evironment with Python 3, MDanalysis, nglview libraries
- Access to Newton cluster with Gromacs+PLUMED installed or install Gromacs and PLUMED at your local workstation. See [http://www.gromacs.org](http://www.gromacs.org) [http://www.plumed.org](http://www.plumed.org)
- We will use mol_model_course_PLUMED conda environment on newton.

## Learning resources
- [A quick introduction to PLUMED](https://www.youtube.com/watch?v=PxJP16qNCYs)
- [Video lecture on MetaDynamics](https://www.youtube.com/watch?v=bZZggbV2r5E)
- [PLUMED manual](https://plumed.github.io/doc-v2.3/user-doc/html/_syntax.html) 



## Assignments

Take an arbitrary alpha-helix from your protein of interest with length of up to 10 aminoacids:


1. Run steered MD where the ends of this helix will we gardually stretched with a moving restrained.
2. Present MD stapshots.
3. Plot of distance between the end C-alpha atoms of the helix with time.


Take the first two amio acids from this helix (a dipeptide).
1. Run  unbiased simulations of the dipeptide.
2. Plot a Ramachandran plot the the phi and psi angles.
3. Perform Metadynamics simulations by biasing phi and psi angles.
4. Make a comparative Ramachandran plot for the two simulations.


### Troubleshooting
- Consult with the seminar protocol/recording
- Ask questions in Slack
