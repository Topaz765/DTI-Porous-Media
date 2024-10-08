# DTI-Porous-Media
Diffusion Tensor Imaging Workbook

# Diffusion tensor

The Diffusion Tensor workbook can be used to perform diffusion tensor imaging within digitized three-dimensional micro-CT data (or other .tif file). The workbook has an input of the desired .tif file and returns a .csv file containing the selected diffusion times, the tortuosity, the matrix components, and the parameters.

#Requirements

The workbook requires the following Julia modules:
IJulia
HTTP
Images
FileIO
Distributed
LinearAlgebra
Distributions
SharedArrays
Random
Measures
Interpolations
HDF5
CSV
DataFrames
Plots

# Installation

The workbook was produced using Julia (more information here: The https://github.com/JuliaLang/julia/tree/master) using the JupyterLab interface (more information here: https://julialang.github.io/IJulia.jl/stable/manual/running/).

# Usage

In order to use the workbook, the user must select the location of their 3D file and insert it into the "# Loading CT data" cell. This is currently set to the example file within the repository. 
The user may then decide on the number of processors to use in the "# Add as many processors as desired" cell.
The user may define their desired parameters in the "# Setting up parameters" tab. This includes the resolution of the 3D image, diffusion coefficient, and the number of molecules to be perform the random walk.
Finally, the user must define the location for the data sets to be saved.
Note: Should the workbook be run without changing the example parameters, the results may differ from those in the test documents since diffusion is a random process and the example structure is not tortuous by nature.

# Producers

The workbook was initially run in Julia version 1.7.1. The workbook was produced as part of a PhD project carried out by Topaz Cartlidge, completed in 2024.


# Maintainers

The workbook is maintained by Giuseppe Pileio (g.pileio@soton.ac.uk) at the University of Southampton, Magnetic Resonance research group.
