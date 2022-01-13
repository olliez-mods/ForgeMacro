# MacroFormatter
Formatter for my macro forge mod

IMPORTANT:
for some features to work (such as loading and saving scripts)
go into your .minecraft folder (found at %appdata%/roaming/.minecraft)
and create a folder called "MacroFiles" this will become an automated 
feature later but until then you MUST create it manuly


How to Use Mod:
the interface is through chat there are several commands you can use such as:

doScript (runs commands typed after it if ther'e seperated by /nl/ eg: "doScript say start/nl/wait 1/nl/say stopped"
  This has a limit of 256 charictors because of minmecrafts chat limit)
  
  #load (loads a script into your MacroFiles folder, "load nameOfScript start/nl/wait 1/nl/say stopped")
  
  #run (runs a script saved in MacroFiles folder, "run nameOfScript")
  
  stop/#stop (stops the current script from running)
  
  #list (lists all scripts)
  
  #del (removes a script)


Scripts are run one command at a time, each command is sepperated by /nl/ to simbolize a new line, using the formatter
you can convert easy to read scripts:

say hi
wait 1
jump
crouch
wait 0.5
stopCrouch
say bye

into functional code:

say hi/nl/wait 1/nl/jump/nl/crouch/nl/wait 0.5/nl/stopCrouch/nl/say bye

if you want a list of all the commands look at the help.txt file


How to Use formatter:
the formatter was made in python and despite what your computer probably says, is not a virus.
It converts, and saves your scripts so you don't have to do it yourself

Layout:
In the initial window there three boxes (well.. one box and two buttons) on the top you'll see a "Copy and Format" button which 
formats your script (by putting those annoying /nl/'s in there) for you and pastes it into your clipboard. Second you'll see a
"Save to Script" button, this pulls up a prompt which asks for a name for your script, when you hit "Save" the script will be
formatted and saves into a txt file in your MacroFiles folder (which again.. is in your .minecraft folder). The third box is
where you write all you code, its written line by line, empty lines and comments (prefixed with a "::"), this is an example:

::greet everyone.\n
say hi\n
wait 1\n

::jump and crouch at the same time.\n

jump\n
crouch\n
wait 0.5\n
stopCrouch\n

::say goodbye ;-;.\n
say bye

