# VSCode-4-Embeded-C
This repository contains information regarding how to setup VS Code(Any Text Editor Just few things will be different) for Embeded C Development.

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
  5. Now Copy paste your make file into the directory.
  6. Change the MakeFile config according to your builb. 
  7. If you need the hex file then remove the burn part.
  8. After configuring the make file- ctrl+shift+p select Tasks:Configure Task Option.
      Now-                                                                                        
        a. remove whole options div.             
        b. remove all the args.                         
        c. change the path inside "command" to "make".                                    
        d. change the lable to anything you like.                                             
        e. <u>Now Run your app by selecting the option with the lable you have given.</u>          
  9. OR simply run by putting make in terminal by navigating to the directory. You dont need to create a task.

## Link to Download AVR Header Files- https://www.nongnu.org/avr-libc/

