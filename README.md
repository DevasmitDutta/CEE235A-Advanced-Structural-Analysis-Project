## This repository contains the user-defined structural analysis routines for analysing structures of any geometry with `MASTAN2` GUI Integration. This project was carried out as course project for 235A Advanced Structural Analysis Course at UCLA.

## Instructions to run the codes

The main routine for running the 3-D 1st order linear-elastic analysis is the `ud_3d1el.m` file. All other files are the sub-routines with independent functionalities such as generating the element level stiffness matrix, force vector depeding on the kind of loading, transforming the local stiffness matrix into global level, releasing the out-of-plane moments at either ends of the member depending on its flexural rigidity at the ends and then post-processing.   

Below is the computation graph of the codebase that demonstrates the overall flow of control across different sub-routines.