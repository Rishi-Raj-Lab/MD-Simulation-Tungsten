# MD-Simulation-Tungsten
Herein, we employ molecular dynamics simulation technique to study the generation of defects during the flash sintering of tungsten. We also study other observables such as phonon dispersion, kinetic energy, diffusion and MSD.


## Simulation Setup and Initialization
The size of the simulation box is 20a x 17a x 20a withthe bottom 20a x 2.5a x 20a set to be immobile
Lattice parameter, a = 3.1648 Å
Boundary is set such that a and c axes have periodic boundary condition imposed on them while b-axis is a free surface

## Potential Energy
The interatomic potentials used - W.eam.fs - in this study is Finnis-Sinclair potential which is the most suitable for a BCC metal like tungsten. The potential was obtained from the NIST repository via https://www.ctcms.nist.gov/potentials/system/W/#W 

## Integration 
Velocity-verlet algorithm was used to track the tracjetories of atoms velocities and positions,  an image was captured after every 5000 steps.
Nose-Hoover chain thermostat to carry out the siimulation at a fixed final temperature attained after equilibration.
The total simulation time is 0.4ns, from a total of 800 000steps and a timsestep of 0.5fs.

## Observables
- Phonon Spectra
- Kinetic energy change with respect to time
- Defect formation
- Mean Squared Displacement
- Diffusion Coefficient
