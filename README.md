# VisualAduitoryModality

# (Preliminary data analysis)
This is my first attempt to analyze the data for my experiment from Psychopy (version 3.1.2)

# About the experiment: 
You will observe an image (blue rectangle) and several different sounds (music) together and you will reproduce their length by pressing 'space' to start and pressing again to stop. Do not press and hold the 'space bar.' During the trials you will shortly see a "+" sign, but you do not have to respond - it just helps you keep your eyes focused on the screen. 

First, you will be asked to focus on either the image or the sound. You will always be presented with both a blue rectangle and music simultaneously (the music pieces will vary). 

Please, pay attention to the duration of  what you have been asked to focus on without counting.  

Match the duration using 'space bar' to start and stop the process.  At this stage you may hear music, see the blue rectangle, or see a blank screen. 


 both stimuli "Visual" and "Auditory" . Then you are going to match the duration of your assigned modality in the estimation phase with the reproduction phase. 

In other words, you are only reproducing what you have attend to. 


Now focus on the image 
Now focus on the sound 

#### From the cvs. Files there are only five columns that we care about: 

# Opening_text	stim_ending_t	visbility	soundvolume	key_resp_2.rt
  
 # Opening_text: This contain the two conditions: Now focus on the image (denoted '0' in excel file) & Now focus on the sound  (denoted '1' in excel file).

# stim_ending_t: These are the six standard time intervals that are randomized through out the experiment.

In the reproduction phase the P will randomly be in only one of these conditionds: 
 # visbility: denoted '1' in excel file which means P see the image. When its '0' they do not see image
# soundvolume:  denoted '1' in excel file which means P hear the music. When its '0' they do not hear the music. 
# blank/empty: means visbility and soundvolume = 0 P DO NOT see or hear anything, just a blank screen.

key_resp_2.rt: This is the reproduction time for all the trails. 


# What am I trying to find here?
	- I am trying to calculate the means of this data frame and group them in a tale (6*4)! I know how to do that using averageifs in excel but because I want to eventually get the standard deviation and coefficient of variation (CV) I need to learn that in R.
	For now I just need the mean. Here are my conditions:
	I need a table where the "stim_ending_t" which is my time intervals are arranged from 1.0 to 3.5 in a rows. For time intervals I need these three conditions to be met while calculating the mean which is "key_resp_2.rt"
	
	only image Visibility and soundvolume(V=1 & s=0)
	
	Only Sound (V=0 & s=1)
	
	Blank (V=0 & s=0)
	
To see an example of how the table should look like see file name "mastersheet_demo_updated" then look within for "Analysis by intervals" sheet.

