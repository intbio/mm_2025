# Workshop: Introduction to Docking

## Description
- We will outline basic methods of docking with AutoDock Vina using Open Drug Discovery Toolkit.
- Duration: 90 minutes
- Objectives: be able to 
    - Understand how to configure docking parameters
    - Convert pdb files to pdbqt
    - Perform docking with AutoDock Vina in Python
    - Perform docking with SwissDock web server
    - Understand and analyse docking results

## Jupyter notebook
- [analyse.ipynb](analysis.ipynb)
- [docking.ipynb](docking.ipynb)
## Required software and resources
- Access to a Jupyter notebook evironment with Python 3, MDanalysis, nglview and oddt libraries
- Access to Newton cluster with MDanalysis, nglview and oddt installed or install MDanalysis, nglview and oddt at your local workstation. See [https://oddt.readthedocs.io/en/latest/rst/oddt.html](https://oddt.readthedocs.io/en/latest/rst/oddt.html)
- Access to SwissDock web server [http://www.swissdock.ch/](http://www.swissdock.ch/)
## Learning resources
- oddt Documentation [https://oddt.readthedocs.io/en/latest/rst/oddt.html](https://oddt.readthedocs.io/en/latest/rst/oddt.html)
- AutoDock Vina Documentation [https://oddt.readthedocs.io/en/latest/rst/oddt.docking.html](https://oddt.readthedocs.io/en/latest/rst/oddt.docking.html)



## Assignments

Perform protein-ligand docking.
1. Select a PDB structure of protein-ligand complex.
2. Save protein and ligand PDB structures into different files (if need).
3. Configure docking parameters.
4. Perform protein-ligand docking via AutoDock Vina and SwissDock.
5. Compare results, visualize best ligand conformations for every method and initial PDB.
6. Calculate RMSDs for best ligand conformations obtained with AutoDock Vina and SwissDock comparing with initial ligand PDB conformation.

### Suggested problem sets
Each student should take a unique PDB structure at his/her own discretion.

### Troubleshooting
- Consult with the seminar protocol/recording
- Ask questions in Telegram
