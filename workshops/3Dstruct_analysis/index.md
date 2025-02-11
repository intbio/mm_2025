# Workshop: Analyzing 3D PDB structures.

## Description
### Part 1.
- Complex analysis of PDB structures
- Duration: 90 minutes
- Objectives: be able to 
    - use Pymol and UCSF Chimera programs for analysis
    - do analysis in Python using MDanalysis and Prody libraries
    - select, extract and analyze atom coordinates and dihedral angles.
    - add hydrogens to the structure

 ### Part 2. 
- identify protonation states
- assign charges to the atoms
- identify hydrogen bonds
- compute and analyze electrostatic surface
- build contact maps
- identify domains
- find homologous structures
- make structural alignment, compute RMSD
- generate sequence alignment from structural alignment
- identify residue conservation
- analyze dynamics using elastic networks models

## Jupyter notebook
- [3Dstruct_analysis.ipynb](3Dstruct_analysis.ipynb)
## Required software and resources
- Pymol, [installation instructions](https://github.com/intbio/mol_model_course/blob/main/workshops/pymol/installation.md)
- UCSF Chimera (optional)
- VMD [installation link](https://www.ks.uiuc.edu/Development/Download/download.cgi?PackageName=VMD) 
- Access to a Jupyter notebook evironment with Python 3
- 3-button mouse

**List of Conda packages:**
- MDanalysis 
- nglview  
- prody 
- propka or use https://www.ddl.unimi.it/vegaol/propka.htm 
- pdb2pqr or use https://server.poissonboltzmann.org/pdb2pqr 

**Channels list (if you use Anaconda Navigator):**
- conda-forge
- schrodinger 

## Learning resources
- MDanalysis tutorial [https://www.mdanalysis.org/MDAnalysisTutorial/](https://www.mdanalysis.org/MDAnalysisTutorial/)
- Prody tutorial [http://prody.csb.pitt.edu/tutorials/prody_tutorial/](http://prody.csb.pitt.edu/tutorials/prody_tutorial/)
- APBS documentation [https://apbs.readthedocs.io/en/latest/](https://apbs.readthedocs.io/en/latest/)


## Assignments

Семинар 3.1. 
0. Загрузите структуру PDB ID 6T78 и посмотрите на струтуктуру с помощью nglview. 
1. С поомщью MDAnalysis опишите какие есть сегменты в структуре, сколько аминокислотных остатков или пар нуклеотидов в каждом из сегментов.
2. Отрисуйте структуру таким образом, чтобы были видны атомы и связи (например, licorice representation).
3. Добавьте водороды в структуру. Отрисуйте новую структуру так, чтобы были видны водороды.
4. Расчитайте длину ДНК. Для эттого для крайних пар нуклеотидов ДНК (внимательно смотрите на нумерацию остатков) найдите координаты центров масс и рассчитайте длину вектора между центрами масс. Ответ принимается с единицами измерения! (см. документацию MDAnalysis) 
5. (сложное) Удлините фрагмент ДНК. Для этого
   - создайте новый объект universe - u2, в котором выберите только ДНК
   - С помощью функции [alignto](https://docs.mdanalysis.org/1.0.1/documentation_pages/analysis/align.html) сделайте выравнивание нижнего края ДНК нового universe объекта (u2) с верхним краем ДНК старого universe объекта (u1), 
   - сделайте [Merge](https://docs.mdanalysis.org/2.7.0/documentation_pages/core/universe.html#MDAnalysis.core.universe.Merge)
(u1.atoms, u2.select_atoms(ВЫБОРКА ДНК).atoms)
   - запишите результат функции Merge в новый PDB файл с помощью функции [write](https://docs.mdanalysis.org/2.7.0/documentation_pages/core/groups.html#MDAnalysis.core.groups.AtomGroup.write).  

Семинар 3.2.
Выберите одноцепочечную белковую структуру на ваше усмотрение.

Для неё:
1. Постройте карту Рамачандрана
2. Постройте карту контактов остатков белка
3. Определите состояния протонирования ионизируемых остатков (сравните модельную и реальную pKa)
4. Визуализируйте электростатический потенциал на поверхности с помощью PDB2PQR и APBS
5. Найдите структуру, родственную Вашей (можно найти в базах SCOPe, PFAM и т.п.)

Для двух гомологичных структур:
1. Сделайте структурное выравнивание, определите RMSD
2. Сделайте выравнивание последовательностей
3. Покрасьте выровненные структуры по консервативности

### Troubleshooting
- Consult with the seminar protocol/recording
- Try to Google, and see Pymol Wiki
- Ask questions in TG
