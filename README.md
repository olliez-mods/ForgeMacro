# ForgeMacro
Formatter for my macro forge mod

This is a minecraft mod that allows you to write scripts in-game to automate stuff

The programing launguage I created has functions, if-statement etc.

Was a super fun project to work on, and also was my first GUI.


At some point I'll add some example scripts to this.

HOW TO USE:

FORMAT OF THE SCRIPTS:
  Each script is saved in your minecraft folder (MacroFiles) and the format is as follows:
    a script is saved in a way that each command is seperated by "/nl/".
    as long as each command is seperated by those charectors you're welcome to create your own editor.

HOW TO USE EDITOR/GUI:
  type the command #e or #edit to access editer it will (hopefully) open a blank page
  you can load files from the MacroFiles folder (in your .minecraft folder)
  it is a bit glitchy as i coded it myself, but your welcome to create your own editor
  It has cool synbtax highligting if you make a comment, a comment line starts with "#" eg. #this block makes you jump 5 times

HOW TO USE WITHOUGHT GUI:
  You can do most things withough the GUI so here are the commands to do so.
  
  #doScript (runs commands typed after it if ther'e seperated by /nl/ eg: "doScript say start/nl/wait 1/nl/say stopped" 
  This has a limit of 256 charictors because of minmecrafts chat limit)

  #load (loads a script into your MacroFiles folder, eg. "load nameOfScript start/nl/wait 1/nl/say stopped")

  #run (runs a script saved in MacroFiles folder, "run nameOfScript")

  #stop/stop (stops the current script from running)



if you want a list of all the scripting commands look at the help.txt file
