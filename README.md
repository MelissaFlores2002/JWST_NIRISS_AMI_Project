# JWST_NIRISS_AMI_Project
Project for space instrumentation, conducting 1st order analysis using the AMI instrument on JWST. This is creating a renormed standard deviation of closure phase and comparing it to a SG FWHM. This work is inspired by: https://iopscience.iop.org/article/10.3847/2041-8213/ad21fb/pdf
\n **All code is in Python

# Functions
There are 7 functions used in this code. All have been made into their own file for readability.
1. MakeFig: Makes a figure of the aperature positions, the intensity of the Point Spread Function, the logrithmic intensity and the crooss section of the logrithmic intsensity. 
2. CreatingAperatures: Makes hexogonal aperatures based on the center locations given to the function.
3. FourierPropagation: Computes the magnitude of the plane after conducting a Fourier transform on the apreature.
4. ClosurePhaseAngleProduction: Takes the centers, aperature mask and the mesh grid and converts them into the closure phase angles by using the baselines of the three centers then find the complex visibilities and phased based on that. Once that is done, it then calculates the phase angle for each baseline, summing them together.
5. CreatingTriangleOnAMI: Creates a plot that shows the triangle of the centers used.
6. InjectPlanet: Simulates an off-axis companion.
7. SuperGaussianFunction: Applies a Super Gaussian window onto the grid, using an equation found in the literature. 

# Main File
The main file is the entire script without the functions in them. There is some redundency due to troubleshooting during the debugging phase, if needed comment those lines out. 

# Slide Deck
Attached there is a slide deck made for my Space Instrumentation class that explains what is conceptually occuring in the code.
**ALL SOURCES OF LITERATURE USED IN ORDER TO MAKE THIS CODE ARE FOUND IN THE REFEREENCES SECTION OF THE SLIDE DECK.  
