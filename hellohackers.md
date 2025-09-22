# INTRO TO COMMANDS

In this challenge, you will invoke your first command! When you type a command and hit enter, the command will be invoked, as so:

hacker@dojo:~$ whoami
hacker
hacker@dojo:~$
Here, the user executed the whoami command, which simply prints the username (hacker) to the terminal. When the command terminates, the shell once again displays the prompt, ready for the next command.

In this level, invoke the hello command to get the flag! Keep in mind: commands in Linux are case sensitive: hello is different from HELLO.

## Solution:

COMMAND USED : hello
output received :
Success! Here is your flag:
pwn.college{A26tLRg3MXAYYF0KceOyDs_Adtd.QX3YjM1wCM2AzNzEzW}

## Flag: 

```
pwn.college{A26tLRg3MXAYYF0KceOyDs_Adtd.QX3YjM1wCM2AzNzEzW}
```


### References:

- [link 1](https://pwn.college)
- 
### Notes:

we can directly invoke commands in linux terminal

# Intro To Arguments

Let's try something more complicated: a command with arguments, which is what we call additional data passed to the command. When you type a line of text and hit enter, the shell actually parses your input into a command and its arguments. The first word is the command, and the subsequent words are arguments. Observe:

hacker@dojo:~$ echo Hello
Hello
hacker@dojo:~$
In this case, the command was echo, and the argument was Hello. echo is a simple command that "echoes" all of its arguments back out onto the terminal, like you see in the session above.

Let's look at echo with multiple arguments:

hacker@dojo:~$ echo Hello Hackers!
Hello Hackers!
hacker@dojo:~$
In this case, the command was echo, and Hello and Hackers! were the two arguments to echo. Simple!

In this challenge, to get the flag, you must run the hello command (NOT the echo command) with a single argument of hackers. Try it now!

## Solution:

command used : hello hackers
output :Success! Here is your flag:
pwn.college{A26tLRg3MXAYYF0KceOyDs_Adtd.QX3YjM1wCM2AzNzEzW}

## Flag: 

```
pwn.college{A26tLRg3MXAYYF0KceOyDs_Adtd.QX3YjM1wCM2AzNzEzW}
```


### References:

- [link 1](https://pwn.college)
- 
### Notes:

this illustrates how to run commands with arguments. the first part is always a command and is followed by argument/s

# Command History

You're going to type a lot of commands, and typing everything from scratch can be annoying. Luckily, the shell saves a history of every command you invoke.

You can scroll through those saved commands with the up/down arrow keys, and we'll practice that in this challenge. This challenge will inject the flag into your history. Bring up a terminal, hit the up arrow, and grab it! In other challenges, the history will contain the log of the commands you've run, so if you need to run a similar command again, you can use the arrow keys to scroll through and find it!

## Solution:

step 1: press the up key repeatedly until flag is visible as a command :

 the flag is pwn.college{kGSfoEeHBb0sCv-uDWcxGyt39rs.0lNzEzNxwCM2AzNzEzW}
 if you press enter by mistake a error will be shown i.e.:
bash: the: command not found

## Flag: 

```
pwn.college{kGSfoEeHBb0sCv-uDWcxGyt39rs.0lNzEzNxwCM2AzNzEzW}
```


### References:

- [link 1](https://pwn.college)
- 
### Notes:

we can use the up and down keys to navigate and reuse the commands previously used saving time from retyping.


