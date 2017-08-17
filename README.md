# Basic-Shell

This is a programming asssignment of the Computer Enginneering course Operating Systems. <br> <br>
The assignment document can be found in the main directory as a pdf file with a name `cse333_project2`

# Instractions that possible to perform
- `ls -l`
- `ls -l <pathname>`
- `gedit`
: 
In the project, foreground and background processes are handled. When a process run in foreground, the shell waits for the task to complete, then immediately
prompt the user for another command.

 - `gedit &`
: 
A background process is indicated by placing an ampersand (’&’) character at the end of
an input line. When a process run in background, the shell does not wait for the task to
complete, but immediately prompt the user for another command.
- `cd <directory>`
- `dir`
- `clr`
: simply "clear"
- `wait` : This is described for background processes. By typing a trailing ampersand (&), the shell knows you just want to launch the
process, but not to wait for it to complete. Thus, you can start more than one job by repeatedly using the trailing ampersand.
Sometimes you will want to wait for processes to complete. To do this, in this
shell you will simply type wait. The built-in command wait should not return
until all background processes are complete.
<br> In this example below, `wait` will not return until the three processes all are
finished.

#### Example
```
gedit &
firefox &
gnome-calculator &
wait
```

- `hist` <br>
This command is for maintaining a history of commands previously issued.
<br>`hist` print up to the 10 most recently entered commands in your shell.
- `hist –set <num>` <br>Set the size of the history buffer to num. (The default value
is 10).
- `! <number>` <br> 
A user should be able to repeat a previously issued command by
typing “! number”, where number indicates which command to repeat.
**Note that “! 1” is for repeating the command numbered 1 in the list of
commands returned by history, and “! -1” is for repeating the last
command**.


- `! <string>` <br>
A user should be able to repeat a previously issued command by typing
`! <string>`, where string indicates the first characters of a most-recent command. If a
user has executed “chmod 777 a.sh” and wants to repeat this command, “! chm”
can be used.
**We were not allowed to use history command of Linux for this command. We
kept them by our own data structures**.

#### Bonus
- `|` : pipe operator
