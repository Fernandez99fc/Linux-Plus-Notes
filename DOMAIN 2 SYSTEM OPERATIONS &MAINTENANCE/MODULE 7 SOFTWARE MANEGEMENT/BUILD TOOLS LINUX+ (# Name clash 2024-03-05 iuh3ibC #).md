OBJECTIVES
--
UNDERSTAND THE BUILD TOPICS COVERED IN THE LINUX+ EXAM..
EXPLAIN THE PURPOSE OF THE "CONFIGURE" COMMAND, "MAKE" COMMAND,COMPILERS AND THE "MAKE INSTALL" COMMAND..

LINUX SOFTWARE INSTALLATION IS GENERALLY DONE THROUGH PACKAGE MANAGERS. 
THERE ARE AT TIMES, YOU WILL HAVE TO INSTALL SOFTWARE FROM SOURCE CODE;
 -WHEN SOFTWARE IS NOT AVAILABLE IN A PACKAGE MANAGER.
-WHEN THE DEVELOPER DOESN'T PROVIDE THE PACKAGE.
-WHEN YOU WANT TO CUSTOMIZE THE INSTALLATION.

EXTRACTING SOFTWARE
--
WE COVERED TAR,TGZ AND GZ PACKAGES. IN LESSON 7.2.
SOURCE CODE WILL PRIMARY COME AS A TAR OR TGZ PACKAGE.

YOU EXTRACT THE FILE USING A TAR COMMAND:
- TAR -xzvf <filename> .tgz - (FOR A GZIP COMPRESSED FILE)
- TAR -xvf <filename> .tar-  (FOR A REGULAR TAR FILE.)

READYING FILES FOR COMPILATION
-----
MOST SOUCRE CODE PACKAGES WILL HAVE A CONFIGURE SCRIPT FILE INCLUDED AND IT IS A COMMAND USED TO SETUP INSTALLATION FILES 
REQUIRED TO COMPILE THE SOFTWARE.
(NOTE: COMPILING REFERS TO THE ACT OF CONVERTING A PROGRAM WRITTEN IN HIGH LEVEL LANGUAGE TO A LOW BINARY LANGUAGE UNDERSTOOD BY THE COMPUTER. TO COMPILE, WE NEED A COMPILER WHICH IS A SOFTWARE PROGRAM USED TO CONVERT FROM HIGH LEVEL LANGUAGE TO MACHINE CODE.)

ONCE THE PACKAGE HAS BEEN EXTRACTED WITH TAR, YOU CAN NAVIGATE TO THE EXTRACTED DIRECTORY TO RUN THE CONFIGURE COMMAND : ./CONFIGURE.

THE CONFIGURE SCRIPT WILL:
- VERIFY ENVIRONMENT IS COMPATIBLE.
- CHECKS TO MAKE SURE A COMPILER IS AVAILABLE (GCC OR GCC-C++)
- CREATES A MAKEFILE.

RUNNING  A COMPILER
--

THE MAKEFILE CREATED IS VERY IMPORTANT TO THIS STEP, IT IS :
- USED TO SPECIALIZE THE SOURCE CODE TO OUR SYSTEM OR THE DITRIBUTION THAT WE ARE RUNNING.
- ENSURING THE APPLICATION WILLL RUN ON YOUR DISTRIBUTION.
- ENSURING THE APPLICATION WILL RUN ON YOUR ARCHITECTURE..

THE NEXT STEP IS TO USE THE "MAKE" COMMAND TO CALL THE COMPILER.
- IT TELLS THE C OR C++ COMPILER TO READ MAKE FILE INSTRUCTIONS.
- THE COMPILER GENERATES A COMPILED EXECUTABLE. 

INSTALLATION
--
NOW THAT WE HAVE THE EXECUTABLE, WE NEED TO INSTALL IT!

HERE WE USE THE MAKE COMMAND AGAIN, BUT WE RUN "MAKE INSTALL"
- MAKE WILL GET INSTALLATION INFO FROM THE MAKE FILE.
- THE APPLICATION WILL BE INSTALLED ON THE SYSTEM.

AT THIS POINT, THE APPLICATION IS READY TO RUN!

