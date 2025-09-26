# 1. Learning from Documentation
The challenge prompted me to use correct argument in my program for getting the flag.

## My Solve
**Flag:** `pwn.college{szJwb1f6yMguJDn4RxztYFOctLx.QX0ITO0wiN0EzNzEzW}`

In the problem statement, it was provided that, by using the correct argument with my command , I can get the flag.
```
hacker@man~learning-from-documentation:~$ /challenge/challenge --giveflag
Correct argument! Here is your flag:
pwn.college{szJwb1f6yMguJDn4RxztYFOctLx.QX0ITO0wiN0EzNzEzW}
```

## What I learned
I learnt the correct usage of programs depends, in a large part, on the proper specification of arguments to them.
Arguments like -a are necessary for proper functioning of commands.

## References
The problem statement was the reference used.
```
The program for this challenge is /challenge/challenge, and you'll need to invoke it properly in order for it to give you the flag. Let's pretend that this is its documentation:

Welcome to the documentation for /challenge/challenge! To properly run this program, you will need to pass it the argument of --giveflag. Good luck!

Given that knowledge, go get the flag!
```

# 2. Learning Complex Usage
The challenge prompted me to know more about arguments and how they work with different commands.

## My solve
**Flag:** `pwn.college{YgcbQGIdB3ZIImcfDVBuxacFlNO.QX1ITO0wiN0EzNzEzW}`

I was provided in the problem statement that arguments can help me get the flag.

```
hacker@man~learning-complex-usage:~$ /challenge/challenge --printfile /flag
Correct argument! Here is the /flag file:
pwn.college{YgcbQGIdB3ZIImcfDVBuxacFlNO.QX1ITO0wiN0EzNzEzW}
```

## What I learned

I learnt the correct usage of programs depends, in a large part, on the proper specification of arguments to them.
Arguments like -a are necessary for proper functioning of commands.


## References
The problem statement provided was used as the reference
```
Here is this level's documentation for /challenge/challenge:

Welcome to the documentation for /challenge/challenge! This program allows you to print arbitrary files to the terminal, when given the --printfile argument. The argument to the --printfile argument is the path of the flag to read. For example, /challenge/challenge --printfile /challenge/DESCRIPTION.md will print out the description of the level!

Given that documentation, go get the flag!
```

# 3. Reading Manuals
The challenge prompted me to use the man command.

## My solve
**Flag:** `pwn.college{8g_-fegqcWl-xyAoHmdK4h7V9iC.QX0EDO0wiN0EzNzEzW}`

I was provided in the problem statement that by using man command I could know about the manual of a command and get the flag.

```
hacker@man~reading-manuals:~$ /challenge/challenge --gfegqc 847
Correct usage! Your flag: pwn.college{8g_-fegqcWl-xyAoHmdK4h7V9iC.QX0EDO0wiN0EzNzEzW}
```

## What I learned
man is short for manual, and will display (if available) the manual of the command you pass as an argument.

Manpages are stored in a centralized database.

The arguments to the man command aren't file paths, but just the names of the entries themselves 

## References
The problem statement provided was used as the reference
```
The challenge in this level has a secret option that, when you use it, will cause the challenge to print the flag. You must learn this option through the man page for challenge!
```

# 4. Searching Manuals
The challenge prompted me to use the man command and search for the flag.

## My solve
**Flag:** `pwn.college{88UIdtAWFDr3zWdM_1HyUsEN0ln.QX1EDO0wiN0EzNzEzW}`

I was provided in the problem statement that by using man command , I can search for the flag.

```
hacker@man~searching-manuals:~$ /challenge/challenge --vog
Initializing...
Correct usage! Your flag: pwn.college{88UIdtAWFDr3zWdM_1HyUsEN0ln.QX1EDO0wiN0EzNzEzW}
```

## What I learned
We can scroll man pages with the arrow keys (and PgUp/PgDn) and search with /. After searching, we can hit n to go to the next result and N to go to the previous result. Instead of /, we can use ? to search backwards!

## References
The problem statement provided was used as the reference
```
Find the option that will give you the flag by reading the challenge man page.

```

# 5. Searching for manuals
The challenge prompted me to find the manpage where my challenge is and then look for the flag.

## My solve
**Flag:** `pwn.college{At4xvZCzRRfsX0SXy7tD04PWdVW.QX2EDO0wiN0EzNzEzW}`

I was provided in the problem statement that by using man man command , I can view the database of manpages and then find my flag.

```
hacker@man~searching-for-manuals:~$ /challenge/challenge --txvzfs 407
Correct usage! Your flag: pwn.college{At4xvZCzRRfsX0SXy7tD04PWdVW.QX2EDO0wiN0EzNzEzW}
```

## What I learned
 man man teaches you advanced usage of the man command itself, and you must use this knowledge to figure out how to search for the hidden manpage that will tell you how to use /challenge/challenge.

 ## Error received
 The txvzfsytdw that I found was the name of the manpage and not a command.

## References
The problem statement provided was used as the reference
```
This level is tricky: it hides the manpage for the challenge by randomizing its name. Luckily, all of the manpages are gathered in a searchable database, so you'll be able to search the man page database to find the hidden challenge man page! To figure out how to search for the right manpage, read the man page manpage by doing: man man!

```

# 6. Helpful Programs
The challenge prompted me to use --help command in order to know more about manpages.

## My solve
**Flag:** `pwn.college{g1-FtBZCx60kcmaOYMHYM6gjw5p.QX3IDO0wiN0EzNzEzW}`

I was provided in the problem statement that by using help command under manpages, I can find my flag.

```
hacker@man~helpful-programs:~$ /challenge/challenge -p
The secret value is: 160
hacker@man~helpful-programs:~$ /challenge/challenge -g 160
Correct usage! Your flag: pwn.college{g1-FtBZCx60kcmaOYMHYM6gjw5p.QX3IDO0wiN0EzNzEzW}



```

## What I learned
Some programs don't have a man page, but might tell you how to run them if invoked with a special argument. Usually, this argument is --help, but it can often be -h or, in rare cases, -?, help, or other esoteric values like /? 

## References
The problem statement provided was used as the reference
```
In this level, you will practice reading a program's documentation with --help. Try it out!

```

# 7. Help for Builtins
The challenge prompted me to use buitin help commands.

## My solve
**Flag:** `pwn.college{McCVCdP8IeJJxbzGl6gDN-uMISR.QX0ETO0wiN0EzNzEzW}`

I was provided in the problem statement that by using builtins and help commands, I can find the my desired program which holds the flag.

```
hacker@man~help-for-builtins:~$ challenge --secret McCVCdP8
Correct! Here is your flag!
pwn.college{McCVCdP8IeJJxbzGl6gDN-uMISR.QX0ETO0wiN0EzNzEzW}

```

## What I learned
Some commands, rather than being programs with man pages and help options, are built into the shell itself. These are called builtins. Builtins are invoked just like commands, but the shell handles them internally instead of launching other programs.

## References
The problem statement provided was used as the reference
```
In this challenge, we'll practice using help to look up help for builtins. This challenge's challenge command is a shell builtin, rather than a program. Like before, you need to lookup its help to figure out the secret value to pass to it!

```
