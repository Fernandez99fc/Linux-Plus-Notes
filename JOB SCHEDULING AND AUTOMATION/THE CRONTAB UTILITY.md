OBJECTIVES
--
UNDERSTAND WHY CRONTAB IS USED
LEARN HOW A CRON TABLE IS SETUP
CREATE CRONTAB ENTRIES

USING CRONTAB
--
AS WE SAID IN THE LAST LESSON, CRON TABLE FILES ARE ONE OF THE PLACES THE CRON DAEMON LOOKS TO FIND SCHEDULED JOBS
CRON TABLES ARE STORED IN THE DIRECTORIES:
/VAR/SPOOL/CRON/<USER NAME> - IN CENTOS
/VAR/SPOOL/CRON/CRONTABS/<USER NAME> - IN UBUNTU.

BUT WHY USE THIS INSTEAD OF THE INTERVAL CRON DIRECTORIES? 
CRON TABLES AND THE CRON TAB COMMAND ARE USED FOR USER SCHEDULED JOBS AND JOBS THAT DON'T FALL INTO ONE OF THE INTERVALS USED BY CRON.

CRON TABLE CONFIGURATION USING CRON TAB
--
REMEMBER:THE CRON JOB DEFINITION CAN BE FOUND IN /ETC/CRONTAB IN ANY DISTRIBUTION.
MEMORIZE THE COLUMN MEANING- IT IS TESTED ON!
USE A MNEMONIC (IF IT HELPS!)
MY HAPPY DAY MAY DAWN - MINUTE, HOUR, DAY OF MONTH, MONTH, DAY OF THE YEAR
A USER CAN CREATE CRONTAB BY RUNNING: CRONTAB -e (e FOR EDIT).
THE CRONTAB IS CREATED USING THE JOB DEFINITION FORMAT TO THE RIGHT 