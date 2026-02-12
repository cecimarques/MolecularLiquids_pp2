Hello :)

Welcome to the supplemental information of our paper "On the origins and predictability of the hydrostatic limit of molecular liquids".
Here goes a file description:


The **folders** **OPLS-AA** and **CGenFF** contain files named compound-ID.dat, which concern each a given compound investigated in the scope of the given force field. The link between a file and a compound can be made via the ID, which matches the index in table S1 of the Supplemental_information.pdf. Each file contains a microstate sampled at 300 K and 1 atm alongside non-bonded and bonded potential parameters for OPLS-AA and CGenFF. We note that the dynamics from which the microstate was sampled was carried out using a thermostat and a barostat, and so the volume of the simulation box, also present in the files, does not necessarily concern the equilibrium value. 

The **lammps.in file** is a sample of a LAMMPS input file used for carrying out the compression in a 0.2 GPa stepwise fashion every 2 ns starting from the microstates sampled at 300 K and 1 atm and going up to 10 GPa. We note that (i) command lines for collecting data to estimate the properties investigated in our work are also present in the script, (ii) the analysis at 300 K and 1 atm requires another script (this one is just for the pressing part), (iii) although the default mixing rules within LAMMPS are the geometric (see https://docs.lammps.org/pair_modify.html), this is changed to the rightful one (i.e. arithmetic) in case a charmm pair_style is used.
