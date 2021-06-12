# OBS-Colorblind-Simulation
A set of LUTs and instructtions to turn OBS into a colorblind simulator

# How to set up
These instructions are on how to set up Open Broadcasting Software (OBS) to functions as a realtime colorblindness simulator and video recorder. OBS is an open source broadcasting and recording software that also has a "projector" fuction, which makes it perfect for realitme visualizations. This tutorial assumes you have no previous knowledge of how to use OBS.

## Step 1: Getting started
To get started we'll need to downoad OBS, which can be found here: https://obsproject.com/ 

We'll also need to download the set of custom LUT images included in this respository. It's recommended to save these in a location where they are not likely to move, for example "*C:\Program Files\obs-studio\data\obs-plugins\obs-filters\LUTs*"


## Step 2: Your first scene
Scenes in OBS are simply compilations of sources and filters. Sources are the way that OBS gets visual information, for instance a "Display Capture" will show anything that is displayed on a given screen.

To start out, we'll need a new scene to work with. Press the '+' button in the bottom left hand corner of the Scenes section, and name your scene. For this example, we'll name it "Tritanopia".

Now we'll need a source. There are a few sources that can be usefull for this application, but in the example we'll be using the Display Capture source.
Add a new source by clicking the '+' button on the bottom left corner of the Sources section, and select 'Display Capture'.

After selecting Display Capture, you should be met with a properties window for the new Display Capture source. If you have more than one monitor, make sure to select the one you desire, then hit OK.

If the preview is currently showing only a portion of your display, and the edges have a diagonal stripe pattern, this is because the source is larger than the canvas. This can be solved by clicking on source and pressing 'Ctrl+F' to fit the source to the scene.

If everything has been done correctly, the preview should be showing an exact replica of your display.

## Step 3: The colorblind filter
Now that we've got a source set up, all we need to do is our filter. To add a filter, select the current scene in the Scenes section and select 'Filters'.

On the filters window, click the '+' button in the bottom left hand corner and select 'Appply LUT'.

We'll need to supply our filter with a LUT, so select the filter from the list and then click 'Browse'. Navigate to the location you saved the LUTs and select one. For this exapmle we'll use "Tritanopia.png". 

After you have selected the file, click 'Close', and you're all done! Now, whenever this scene is selected in OBS, the preview will show your display with simulated colorblindness!

## Additional Notes:
A super useful feature when using OBS this was is the "projector" function. This can be accessed by right-clicking anywhere in the cavas and selecting either 'Fullscreen Projector' or 'Window Projector'.
