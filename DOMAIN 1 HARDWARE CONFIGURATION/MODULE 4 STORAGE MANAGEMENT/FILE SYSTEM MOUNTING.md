OBJ
-
USE THE MOUNT AND UMOUNT COMMANDS.
UNDERSTAND HOW TO FIND INFORMATION ABOUT MOUNTED FILE SYSTEMS USING /PROC/MOUNT AND /ETC/MTAB.

MOUNTING FILE SYSTEMS
--
NOW THAT WE KNOW HOW TO CREATE FILE SYSTEMS. HOW DO WE ACCESS IT?
THE PROCESS OF MAKING A FILE SYSTEM AVAILABLE FOR USE AND MAKE IT ACCESSIBLE IS CALLED MOUNTING A FILE SYSTEM.

TO SEE IF A FILE SYSTEM HAS BEEN MOUNTED ON A DEVICE, YOU CAN GREP:
MOUNT | GREP SD.
TYPING THE MOUNT COMMAND WILL SHOW ALL MOUNTED FILE SYSTEMS ON THE SYSTEM.

TO MOUNT A FILE SYSTEM, WE WILL CREATE THE MOUNT AND GIVE IT A NAME IN /MNT- WHERE WE WILL MOUNT IT.
MKDIR /MNT/EXT4 /MNT/XFS.
AFTER CREATING.
MOUNT THE PARTITION WITH THE EXT4 FILE SYSTEM INTO THE FILE SYSTEM DIRECTORY:
MOUNT /DEV/SDB1 /MNT/EXT4.

MOUNT COMMAND READS FROM THE /PROC/MOUNT FILE.
YOU CAN ALSO CAT /PROC/MOUNTS INSTEAD OF RUNNING THE MOUNT COMMAND.
WE CAN ALSO THE READ THE /ETC/MTAB(MOUNT TAB)

UNMOUNTING FILE SYSTEM
--
WE USE THE UMOUNT COMMAND TO UNMOUNT A FILE SYSTEM.
UMOUNT /MNT/EXT4
UMOUNT /MNT/XFS

