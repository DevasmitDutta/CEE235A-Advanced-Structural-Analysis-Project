## This repository contains the user-defined structural analysis routines for analysing structures of any geometry with `MASTAN2` GUI Integration. This project was carried out as course project for 235A Advanced Structural Analysis Course at UCLA in Fall'23.

## Instructions to run the codes

The main routine for running the 3-D 1st order linear-elastic analysis is the `ud_3d1el.m` file. All other files are the sub-routines with independent functionalities such as generating the element level stiffness matrix, force vector depeding on the kind of loading, transforming the local stiffness matrix into global level, releasing the out-of-plane moments at either ends of the member depending on its flexural rigidity at the ends and then post-processing. 

Below is the computation graph of the codebase that demonstrates the overall flow of control across different sub-routines.

![final flow chart](https://github.com/DevasmitDutta/CEE235A-Advanced-Structural-Analysis-Project/assets/76597282/ffe294da-6341-456f-85e7-d5f4403dba92)

The results of the user-defined routine have been validated against the in-built MASTAN2 routine. Different test cases have solved considering different geometry, boundary constraints and loading conditions. All of these examples are included as `.mat` files in the [validation files folder](https://github.com/DevasmitDutta/CEE235A-Advanced-Structural-Analysis-Project/tree/main/Submission/validation%20files). The comparisions have been showed in the [verification problems pdf](https://github.com/DevasmitDutta/CEE235A-Advanced-Structural-Analysis-Project/blob/main/Submission/Final%20Submission/Verification%20Problems.pdf)