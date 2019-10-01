# Circuit Simulation Algorithms CE530 #

Implementation of a state-of-the-art SPICE-like simulation tool, that can simulate efficiently and fast, very large circuits with hundreds of thousand of nodes and simulation variables.

## Features ##

The simulation tool provides the following operations/analyses:

* **DC analysis**
    * direct methods (LU, Cholesky)
    * iterative methods (Bi-/Conjugate Gradient)

* **Transient analysis**
    * Backward Euler
    * Trapezoidal method

* **AC analysis**
    * direct methods (LU, Cholesky) with complex numbers 
    * iterative methods (Bi-/Conjugate Gradient) with complex numbers

Additionally, the simulation tool can make use of **SPARSE** matrices in order to handle very large circuits in memory.

## Dependencies ##

This project requires `GSL` library to be installed for **C**.  
In order to plot the transient analysis `matplotlib` for **python** is also required.


You can install them by issuing the following command to the Makefile:

```bash
make deps
```

or  manually

```bash
1. sudo apt install libgsl0-dev
2. sudo apt install python-matplotlib
```
