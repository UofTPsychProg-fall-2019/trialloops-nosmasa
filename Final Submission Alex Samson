#!/usr/bin/env python3
# -*- coding: utf-8 -*-
"""
Build a trial loop Step 2
Use this template to turn Step 1 into a loop
@author: katherineduncan
"""

#This a short version of the Stroop experiment. 
#The experiement has no time constraints whereby the participant has as much time to answer. 
#The participant is required to hit the key on the keyboard that corresponds to the first letter of the colour that the physical word is
#in NOT the name of the colour that is printed. 
#The participant can only hit one of the four keys to proceed to the next round (either: r,g,b,y corresponding to red, green, blue, and yellow).
#This experiment is designed for geriatrics because they are able to move at their own pace. 

#%% Required set up 
# this imports everything you might need and opens a full screen window
# when you are developing your script you might want to make a smaller window 
# so that you can still see your console 
import numpy as np
import pandas as pd
import os, sys
from psychopy import visual, core, event, gui, logging

stim =['redred.png','yellowgreen.png','yellowblue.png','greenyellow.png']
#correct_answer= ['r','g','b','y']


#loop begins 
for x in range(len(stim)):
    #first window
    win = visual.Window(size=(1536,864), allowGUI=False, color='white')
    text=visual.TextStim(win=win,text="""For each image you are presented tap the key that corresponds to the colour of the word:
    g = green, b = blue,
    r = red, y = yellow.
    When you are ready to begin press the SPACE bar""",pos=(0,0),color='black')
   
    text.draw()
    
    win.flip()
    keys = event.waitKeys(keyList =['space'])
    
    #stimuli 1
    file = r'C:\Users\asamson\Desktop\Stroop\redred.png'
    current_stim = visual.ImageStim(win, image=file, pos=(0,0))
    text=visual.TextStim(win=win,text="""Tap the key that corresponds to the colour of the word:
    g = green, b = blue,
    r = red, y = yellow""",pos=(0,-.7),color='black')
    
    current_stim.draw()
    text.draw()
    
    win.flip()
    keys=event.waitKeys(keyList=('g','b','r','y'))
    print(keys)
    
    #stimuli 2
    file = r'C:\Users\asamson\Desktop\Stroop\yellowgreen.png'
    current_stim = visual.ImageStim(win, image=file, pos=(0,0))
    text=visual.TextStim(win=win,text="""Tap the key that corresponds to the colour of the word:
    g = green, b = blue,
    r = red, y = yellow""",pos=(0,-.7),color='black')
    
    current_stim.draw()
    text.draw()
    
    win.flip()
    keys=event.waitKeys(keyList=('g','b','r','y'))
    print(keys)
    
    #stimuli 3
    file = r'C:\Users\asamson\Desktop\Stroop\yellowblue.png'
    current_stim = visual.ImageStim(win, image=file, pos=(0,0))
    text=visual.TextStim(win=win,text="""Tap the key that corresponds to the colour of the word:
    g = green, b = blue,
    r = red, y = yellow""",pos=(0,-.7),color='black')
    
    current_stim.draw()
    text.draw()
    
    win.flip()
    keys=event.waitKeys(keyList=('g','b','r','y'))
    print(keys)
    
    #stimuli 4
    file = r'C:\Users\asamson\Desktop\Stroop\greenyellow.png'
    current_stim = visual.ImageStim(win, image=file, pos=(0,0))
    text=visual.TextStim(win=win,text="""Tap the key that corresponds to the colour of the word:
    g = green, b = blue,
    r = red, y = yellow""",pos=(0,-.7),color='black')
    
    current_stim.draw()
    text.draw()
    
    win.flip()
    keys=event.waitKeys(keyList=('g','b','r','y'))
    print(keys)
    
    #last window
    file = r'C:\Users\asamson\Desktop\Stroop\2.jpg'
    current_stim = visual.ImageStim(win, image=file, pos=(0,0))
    text=visual.TextStim(win=win,text="THE END",pos=(0,-.2),color='black')
    
    current_stim.draw()
    text.draw()
    
    win.flip()
    core.wait(2)
    
win.close()
print(keys)
