# VSCode-4-Embeded-C
This repository contains information regarding how to setup VS Code for Embeded C Development.

## Instructions-
  1. Setup a workspace in the directory you are writing the code.
  2. Press ctrl+shfit+p and select the option to Edit c_cpp_properties.json file.
  3. If the PORT commands are not recognised go to the defination of avr/io header file
     and the search the name of the board you want to use. 
  4. Now Define the name give inside the curly parentheses in the header of your code.
      eg- 1. #ifndef __AVR_ATmega8__
                #define __AVR_ATmega8__
             #endif
          2. #define __AVR_ATmega8__
  5. Now Copy paste your make fule into the directory.
  6. Change the MakeFile config according to your buil. 
  7. If you need the hex file then remove the burn part.
  8. After configuring the make file- ctrl+shift+p select Tasks:Configure Task Option.
      Now-
        a. remove whole options div.             
        b. remove all the args.                         
        c. change the path inside "command" to "make".                                    
        d. change the lable to anything you like.                                             
        e. <u>Now Run your app by selecting the option with the lable you have given.</u>                                      

### Link to Download Header Files- https://sourceforge.net/projects/winavr/

