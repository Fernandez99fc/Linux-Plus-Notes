UNDERSTAND THE ACQUISITION COMMANDS.
USE TOOLS LIKE WGET AND CURL

ACQUISITION COMMANDS ARE USED IN LINUX TO DOWNLOAD A FILE OR PACKAGE FROM A REMOTE SOURCE.
FOR THE LINUX+ EXAM, THERE ARE TWO ACQUISITION COMMANDS TO KNOW; WGET AND CURL.

WGET
--

THE WGET COMMAND CAN BE USED TO DOWNLOAD PACKAGES AND FILES FROM REMOTE SERVERS VIA;
HTTP
HTTPS
FTP
FTPS.

PRIMARILY, WGET IS USED  AS A SIMPLE WAY TO DOWNLOAD A PACKAGE, WITH THE SYNTAX: WGET <URL OF PACKAGE TO DOWNLOAD>

CURL
-------------------
THE CURL COMMAND WORKS MUCH MORE LIKE WGET BUT HAS MORE FEATURES AND SUPPORTS MORE PROTOCOLS..
TO USE CURL TO DOWNLOAD A PACKAGE OR A FILE LIKE WGET:
CURL -O <URL OF FILE OR PACKAGE TO DOWNLOAD>

ALTERNATIVELY, IF YOU WANT TO SPECIFY A FILENAME:
CURL -o <filename> <url of file or package to download>