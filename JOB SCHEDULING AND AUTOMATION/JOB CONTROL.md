OBJECTIVES
--
UNDERSTAND WHY JOB CONTROL IS IMPORTANT.
LEARN THE WAYS JOBS ARE CONTROLLED

THE PURPOSE JOB CONTROL
--
WHAT CAN YOU DO TO PREVENT A JOB FROM TYING UP YOUR SHELL OR TERMINAL SESSION?
YOU CAN START A JOB IN THE BACKGROUND
WHAT IF YOU KICK OFF A JOB AND YOU WANT TO CANCEL IT?
YOU CAN SEND AN INTERRUPT SIGNAL
WHAT IF YOU WANT TO PAUSE A JOB?
YOU CAN SEND A STOP SIGNAL.
WHAT IF YOU WANT A PROGRAM TO RUN AFTER WHEN YOU LOG OUT?
YOU CAN SEND A NO-HANG UP SIGNAL.

JOB CONTROL BACKGROUND AND FOREGROUND
--
WE SENT A PROCESS TO THE BACKGROUND WITH THE AMPERSAND(&):
SOMESCRIPTS.SH &
TO SEE THE JOBS RUNNING IN THE BACKGROUND,WE CAN TYPE THE JOBS COMMAND:

WE CAN BRING THE BACKGROUND JOB BACK TO FOREGROUND WITH THE FG COMMAND:
FG <JOB ID>

JOB CONTROL COMMANDS: CTRL-C
--
WHEN YOU'RE RUNNING A PROCESS OR JOB ACCIDENTALLY OR YOU JUST WANT TO EXIT OUT OF A LONG-RUNNING JOB, YOU CAN USE CTRL-C
CTRL-C IS ALSO KNOWN AS SIGINT; IT SENDS A SIGNAL INTERRUPT TO THE RUNNING PROCESS, TELLING IT TO QUIT.
SIGINT IS ALSO KNOWN AS PROCESS 2.

JOB CONTROL COMMANDS:CTRL-Z
--
WHEN A JOB HAS TAKEN OVER THE TERMINAL AND YOU DONT WANT TO CANCEL IT, YOU CAN PAUSE THE JOB WITH CTRL-Z.
CTRL-Z IS ALSO KNOWN AS SIGSTOP(PROCESS SIGNAL 19).
STOPS ANY PROCESS RUNNING IN THE SHELL BUT DOES NOT TERMINATE THE PROCESS(THAT'S SIGINT): IT LEAVES THE PROCESS IN MEMORY.
FROM HERE YOU CAN MOVE THE JOB INTO THE BACKGROUND WITH THE BG COMMAND.
THE JOB WILL CONTINUE TO RUN BUT NOT IN YOUR TERMINAL.
SIMILAR TO RUNNING A PROCESS IN THE BACKGROUND BY USING AN &
WE CAN BRING THE PROCESS TO FOREGROUND WITH FG, SAME AS BEFORE.

JOB CONTROL COMMANDS:NO HANG UP(NOHUP)
--
WHEN YOU LOG OFF A SHELL TERMINAL SESSION, A SIGNAL UP IS SENT (SIGHUP -PROCESS SIGNAL 1)
IT CLEANS UP ALL PROCESSES LEFT BY THE TERMINAL SESSION.
HOWEVER, YOU CAN TELL A SYSTEM NOT TO RUN SIGHUP ON CERTAIN PROCESSES 
- THIS LEAVES THE PROCESSES RUNNING EVEN AFTER YOU LOG OFF.

YOU DO THIS WITH THE NO HANG-UP COMMAND,OR NOHUP:
NOHUP SOMESCRIPTS.SH &
IN THE EXAMPLE ABOVE, THE SCRIPTS WILL RUN IN THE BACKGROUND EVEN IF YOU LOG OUT.
