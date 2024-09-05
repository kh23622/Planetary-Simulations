# Welcome to the Planetary Simulation with HERCULES
## Description

#### This README provides clear and simple steps to help you run and build an Earth-like planet using the HERCULES simulation framework. Follow the instructions to set up the environment, configure the input files, and explore the detailed output from the simulation. Whether you're a first-time user or an experienced researcher, this guide will ensure you can model planetary systems with ease.

### Prerequisites:
#### STEP 1: Fork and Clone the HERCULES Repository by using below link
#### [HERCULES_Development] (git@github.com:sjl499/HERCULES_development.git)

#### STEP 2: Create a new folder with [your_preferred_name]
#### STEP 3: Using 'cp path/to/file1 path/to/file2 /path/to/temp/location/' command on command line, copy the Input files, Analytical Script and EOS files from Tutorial_beta, Make file from Source Code.
This ensures that you have all the files rquired in same path as they are in one directory 

#### Alternative: You can directly run the code from the Cloned repository
In this you will have to edit each file path as the files are in different folder.

##### Ensure you have all the necessary EOS files, Analytical Script files, Input files
#### Create a folder named Output in the same directory
this is where HERCULES will place the output files.

### Prepare Input Files
##### Rename your 'tutorial1.txt' file to 'HERCULES_input.txt' if you're using that example.
this is a file for non-rotating planet. For rotating planet use tutorial2.txt or tutorial3.txt
#### Change the file path of EOS to where it is located in your computer
make sure to verify the paths to the EOS files in the input file, if the run is significantly slower than expected

### RUN the file
#### use command ./HERCULESv1.0 > output.txt
if this says Permission Denied, because the script is non-excuetable. We need to change it to exceutable so we  
#### use command chmod +x HERCULESv1.0 and then rerun the command ./HERCULESv1.0 > output.txt
it may take a few minutues to run the file. 

Once these steps are complete, you will have successfully run HERCULES using the provided example.

To continue with the HERCULES tutorial and work with the output data, follow these steps to extract information and plot profiles:

#### STEP 4: Extract Information Using Python Scripts
###### read_HERCULES_output.py: This script is used to extract information from the output file. You need to modify this script to work with the output file you generated (e.g., tutorial1_L0_N50_Nm400_k6_f020_p10_l10_final_0).
make sure you choose the output file with highest number as it is the last completing all the iterations. this will allow you to see the graph for the planet.


#### STEP 5: Plot profiles using 
##### run command line ./python3 plot_HERCULES_structure.py

