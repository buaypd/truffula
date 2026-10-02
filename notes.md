# Truffula Notes
As part of Wave 0, please fill out notes for each of the below files. They are in the order I recommend you go through them. A few bullet points for each file is enough. You don't need to have a perfect understanding of everything, but you should work to gain an idea of how the project is structured and what you'll need to implement. Note that there are programming techniques used here that we have not covered in class! You will need to do some light research around things like enums and and `java.io.File`.

PLEASE MAKE FREQUENT COMMITS AS YOU FILL OUT THIS FILE.

## App.java
App.java uses the TruffulaOptions Object and the other classes, specific options based on the behavior is needed. Looks like i would need to use a scanner to deterimine the output.

## ConsoleColor.java
This class holds all the color we need to identify the files. 
Q. What will the colors represent in the tree, or can we choose any colors what want to represent our tree.

## ColorPrinter.java / ColorPrinterTest.java
ColorPrinter.java, ColorPrinter object appears to how to color appears in the termial, if to reset to a default color or currentColor(the desired color wanted). What is deteriming the color output?? The User in the termial with a scanner? ColorPrinterTest.java: Tests if the print statment is the desired output, and does it reset, I should test if the Color doesnt not want to reset, does it have the correct color and does it maintaian the same color.

## TruffulaOptions.java / TruffulaOptionsTest.java
TruffulaOptions Object holds the behavior on what is displayed, what's being displayed root file and sub root files, if we want to print out the hidden files or not, and if we need to show use color or not color. TruffulaOptionsTest test what and how its being displayed. The test seems mimnial. We need a test when we only have the path ['/path/to/directory'] and nothing else to see if its not showing hidden files and it if it shows color by default. And also test if we mess with the order it should still behave as intended becuase order DOES NOT matter ['-nc', '-h'] or ['-h', '-nc'].

## TruffulaPrinter.java / TruffulaPrinterTest.java
TruffulaPrinter uses the TruffulaOptions class to help deterime out the tree(files) is printed and the Conslosecolor and colorPrinter for the desired color. Seems like this is where we delare the tree structure for the files and what order it prints into the console  

## AlphabeticalFileSorter.java