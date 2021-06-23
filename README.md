# ARP-ASSIGNMENT-3
# S5058220 RAKESH MOTAMARRI

Simple iteration of the dining philosophers problem, using only IPC  and not used pipes and signal.
# REQUIREMENTS
The program requires the software "konsole" to be installed in order to open up new shell windows to
execute the subprocesses in.

code.c
The file consists of complete program.The main variables are child and parent 
The process is what corodinates the access to the shared resources,represented by the "child".
it is an unended loop,by first checking the child is ready with the fork,then start the process of assessing to ready for the parent then it is readonly process.in between check the failure,read until the end of the process.if the child is not holding the fork notify the parent at once and exit.
The process opens up in write only mode.
The child by writing a placeholder character in a requested info. It then closes and reopens it in readonly mode, waiting for a response.
answer from the _parent_ which is writes on the same pipe as defined.

