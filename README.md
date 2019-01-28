# Creating-own-shell-in-C

This program will write your own shell program, Mav shell (msh), similar to
bourne shell (bash), c-shell (csh), or korn shell (ksh). It will accept commands, fork a child
process and execute those commands. The shell, like csh or bash, will run and accept
commands until the user exits the shell

The program will do the follwing

1. print out a prompt of msh> when it is ready to
accept input. It must read a line of input and, if the command given is a supported shell
command, it shall execute the command and display the output of the command.

2. If the command is not supported your shell shall print the invalid
command followed by “: Command not found.”

3. If the command option is an invalid option then your shell shall print
the command followed by “: invalid option --” and the option that was invalid as
well as a prompt to try —help. exec() will give you this output make sure you pass it
on to your user.

4. After each command completes, your program shall print the msh>
prompt and accept another line of input.

5. Your shell will exit with status zero if the command is “quit” or “exit”.

6. If the user types a blank line, your shell will, quietly and with no other
output, print another prompt and accept a new line of input.

7. support pipes: “|”.

8. support suspending the process with ctrl-z

9. shall background a suspended process with bg

10. support and execute any command entered. Any
command in /bin, /usr/bin/, /usr/local/bin/ and the current working directory
is to be considered valid for testing.
Your shell shall search in the following PATH order:
1. Current working directory,
2. /usr/local/bin
3. /usr/bin
4. /bin
Parameters may also be combined. For example, ps may be executed as: ps –aef or ps
–a –e -f
