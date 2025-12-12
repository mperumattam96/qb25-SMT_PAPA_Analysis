# Analyzing Single-Molecule Tracking Data Obtained by PAPA in Live Cells  

## Description
Single-molecule imaging provides a powerful way to observe molecular interactions in live cells, but it is challenging to track single molecules while also detecting their interactions. Single-molecule tracking (SMT) using proximity-assisted photoactivation (PAPA) is a new technique at allows for visualization of molecular interactions in vivo, using the properties of fluroescent dyes. PAPA in live cells generates vast data sets. The amount of data created through these SMT experiments immediately doubles when working with multiple channels on a microscope. Moreover, this method requires the use of a direct reactivation control in order to normalize the number of proximity activated molecules against the total number of molecules of the given type (e.g., a particular protein—in this case BRD4). As such, we propose creating a Python script that would allow for plotting of localization number as a function of frame number. That is, a program that would permit relating the number of single-molecule trajectories to the live imaging frame number. This script could then be used for the aforementioned normalization.  
https://doi.org/10.7554/eLife.76870

## Example of a Published Figure  
![project_example_figure](https://github.com/user-attachments/assets/357f9478-5547-4736-ad6a-6e8b3d86faf6)  
Calculation of the proximity index. The total number of localizations in each frame are counted before and after violet and green light pulses. In our project, the data we will be using will use spontaneous fluorescence instead of violet-reactivated localizations.  


## Datasets  
Data kindly provided by Thomas Graham and Nicholas Alagna. Example data in "data" subdirectory.   

## Software Versions  
Python v3.12.3 https://www.python.org/.   
* NumPy   
* argparse      
R v4.4.1 https://www.r-project.org/  
* tidyverse  
* ggplot  

## Goals
Main goal: Using a Python script, read in the CSV file obtained from SMT data and tabulate the number of localizations per frame. We will begin with a CSV file that is based on segmentation from a single cell, and focus on columns x, y, frame, and trajectory.  
Stretch Goal 1: Adding onto goal one, factor in background from spontaneous activation. We will extrapolate spontaneous activation after the green light pulse and perform background subtraction.  
Stretch Goal 2: We will look to see if PAPA signal correlates to other properties in the cell. These other properties come from cell segmentation data.    

## Final Presentation 
https://docs.google.com/presentation/d/18htI1pPVnuaStuEToq8l2orn6DnJS3FLkf-jiLvnork/edit?usp=sharing