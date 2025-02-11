# Workshop: Setting up and running simulations in Gromacs

## Description
- We will prepare a protein solvated in water for simulations and run simulations in Gromacs
- Duration: 90 minutes
- Objectives: be able to 
    - Prepare a protein stucture for MD simulations.
    - Solvate structure and add ions.
    - Generate topology and force field parameters.
    - Set up minimization and equlibration parameters
    - Do quality control of structure.
    - Run minimization and equlibration.
    - Set up simulations parameters.
    - Prepare tpr files.
    - Run simulations.

## Jupyter notebook
- [MD.ipynb](MD.ipynb)

## Required software and resources
- Access to a Jupyter notebook evironment with Python 3, MDanalysis, nglview libraries
- Access to Newton cluster with Gromacs installed or install Gromacs at your local workstation. See [http://www.gromacs.org](http://www.gromacs.org)

## Learning resources
- Short Gromacs tutorial [https://github.com/intbio/MolModEdu/tree/master/GROMACS/beginner](https://github.com/intbio/MolModEdu/tree/master/GROMACS/beginner)
- Extended Gromacs tutorial [https://github.com/intbio/MolModEdu/tree/master/GROMACS/nucl](https://github.com/intbio/MolModEdu/tree/master/GROMACS/nucl)



## Assignments

Perform a short MD simulation for a protein of your choice in Gromacs. Short one-chain proteins are preferred.
Expect, that an arbitary chosen protein structure may not be well suited for straightforward
simulations. It may have partially unresolved residues, ligands, etc. Seek advice in advance via Telegram.

1. Present snapshots of system before and after simulations.
2. Include plots of energy, temperature, box size versus simulation time.
3. Prepare another system with your protein in rectangular box with walls ratio 3:1:1. The protein should be placed near one of the walls (not in the center of the box). Add water (any model except TIP3P) and ions (KCl) with 200 mM concentration. Describe your actions in detail.


### Suggested problem sets
Each student should take a unique PDB structure  at his/her own discretion.

### Troubleshooting
- Consult with the seminar protocol/recording
- Ask questions in Telegram
