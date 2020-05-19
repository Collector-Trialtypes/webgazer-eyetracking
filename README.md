<!--
    Collector (Garcia, Kornell, Kerr, Blake & Haffey)
    A program for running experiments on the web
    Copyright 2012-2016 Mikey Garcia & Nate Kornell


    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License version 3 as published by
    the Free Software Foundation.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program.  If not, see <http://www.gnu.org/licenses/>

	Kitten release (2019-20) author: Dr. Anthony Haffey (a.haffey@reading.ac.uk)
-->
# Webgazer-eye tracking

*This is based on code from OSF repository https://osf.io/jmz79/ that accompanies the publication "Online webcam-based eye tracking in cognitive science: a first look" by Semmelmann & Weigelt, published in Behavior Research Methods in 2017.*
  
*Updates by Anthony Haffey (a.haffey@reading.ac.uk) 2020 to make this a freeviewing task that works on Collector*

An eye-tracking trialtype that uses the participant's webcams to track their eye-movements.
Optimised for Collector (go to https://some-open-solutions.github.io/ocollector/ to use without installing).
To make this trialtype work without collector, take note of the "{{" "}}" variables which need to change every trial.

To download the whole experiment right click on

__Placeholder__

and click "save link as". 

Similarly, to save just the trialtype right click on 

__Placeholder__

and click "save link as".

Relevant columns:
- calibrations: The default is 13 calibrations to make the participant look at all 13 predefined points on the screen
- freeview_image_file: Specify where the file is that lists the file locations of the images you are presenting. **Note that for eye-tracking you only have one row in your *procedure* sheet for all the eyetracking trials.**
- design_type: either "freeview" to compare gaze to pairs of images, "simple" to measure participants looking at a dot, or "pursuit" for participants to follow a dot and its movement.
- calibration_skip: Allows you to skip calibration. Just write "skip","on" or "true" in this column to skip. This can be helpful when you're designing experiments.
- image_height: we'd suggest you use px (pixels) rather than % (percentages) to make the stimuli consistent between participants.
- image_width: we'd suggest you use px (pixels) rather than % (percentages) to make the stimuli consistent between participants.
- save_script: unless you are only running the experiment on your local machine, you will need to set up a google script to save your data. This repository comes with "GoogleScript.js", which you need to upload to your google drive as a "Google Apps Script" and then publish to get the location of the script. **NOTE DO NOT DO THIS WITH A PERSONAL GOOGLE ACCOUNT! This script allows participants to write into your google drive! If you haven't already, create a new google account for your research.** Instructions about uploading google scripts can be found at https://docs.google.com/document/d/1SKYIJF1dAjMDS6EHUIwfZm2KQVOzx17S6LbU_oSGxdE/edit?usp=sharing
- trials: How many of the rows in the **freeview_image_file** do you want to run/select?

# Licensing
This code is free to use without restriction, with the same licensing intentions as Collector originally created by Mikey Garcia (https://github.com/gikeymarcia/Collector), currently developed by some open solutions (https://github.com/some-open-solutions/collector):

Collector (Garcia, Kornell, Kerr, Blake & Haffey)
A program for running experiments on the web
Copyright 2012-2016 Mikey Garcia & Nate Kornell


This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License version 3 as published by
the Free Software Foundation.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>

Kitten release (2019-20) author: Dr. Anthony Haffey (a.haffey@reading.ac.uk)
