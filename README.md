# WirelessLinkCharacterization
In this project, we publish empirical data from an experiment campaign. In this campaign, we characterize the link properties considering a ground level deployment.


In this file, i describe how to use data collected during the large experiment campaign we conduted during my PhD Thesis.


I) Requirements
 -- Python 2.7
 -- Python libraries : matplotlib (Plot Figures), 

II) Content of the directory
1) run.sh : Parse data and plot all figures
2) PythonCode : A directory containing all Python file
3) Log files
4) A directory containings images included in the Paper
A) Flat deployment
Extention/$Channel$/MSG/$distance$/$s$.data : The path to log file mask. In this path, parameters are indicating by $$.
	-- $channel$ : Indicates the Channel (11, 14, 18, 22, 26)
	-- $distance$ : The distance between two consecutove sensors
	-- $sensor$ : The log of messages received by sensor N° s
	-- For instance, we can have the path Extention/26/MSG/3/2.data : The messages received by sensor 2 in an experiment with a distance of 3m between consecutive nodes. In this experiment, sensor use channel 26. 
	-- In directory Extention/$Channel$/MSG/$distance$, the maximul value of s indicates the number of sensors used in the experiment.

B) Deployment at height
	-- Extention/$Channel$/Hauteur/MSG/$distance$/$s$.data

C) Deployment on a hill
	-- Extention/$Channel$/Coline/MSG/$distance$/$s$.data

III) To parse file and plot figures
1) Move to the current directory : use the "cd" command
2) run the command "./run.sh"

After runing the previous command, you will see the following directories :

1) Impact_Ground : All the images showing the impact of the ground
2) Impact_MSize : All the images showing the impact of the message size
3) Impact_Channel :  All the images showing the impact of the communication channel
4) Impact_Topograpy :  All the images showing the impact of the topography
5) Distance_Correlation : Images showing the correlation between the link quality and the distance
6) Paper_Images : All the images used in the paper
7) Analytical : Theoretical RSSI and PRR
8) Analytical_Validation : Theoretical validation of empirical data

