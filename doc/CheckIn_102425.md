#First Project Check-In 10242025  

##Prior Feedback   
During our initial meeting, we made sure we had deliverables to ensure progress was being made. We will not be converting the imaging data ourselves, but use the csv file generated from the experimental microscopy data. Our first goal was reasonable, and our stretch goals expanded on that.   

## Progress   
We have completed Goal 1! We utilized three python packages (numpy, pandas, and matplotlib.pyplot) and will not be using R for plotting. Nicholas’s experiment involves tracking BRD4 with and without an HDAC inhibitor and seeing its effects. The csv file we analyzed is this experiment before adding the inhibitor. We read in the data from this experiment, and generated a general practice plot with our data using the plt.plot function. Then we separated each unique trajectory by frame, and plotted frame number on the x-axis and number of trajectories on the y-axis. The data looks as expected, as frame 250 is when the sample experienced the pulse.   

## Project Organization   
We have uploaded the csv file of the data we are analyzing in the data directory (PAPA_0000_0000_trajs.csv). This is data Nicholas collected himself. We have uploaded our current progress on the code in the code directory (Project_Work.ipynb).  

##Struggles/Questions  
As we have successfully completed Goal 1, we are trying to create a script that has a for loop to iterate through multiple files to perform the same function as we did for Goal 1, so we might need help with this next step. The glob module allows us to select all files of the same kind (in our case csv) in the same folder and run the script on it. From that, we will be able to then make plots of the ratio of trajectories/frame for PAPA to spontaneous reactivation.  

