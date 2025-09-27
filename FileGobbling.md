# 1. Matching with *
The challenge prompted me to * globbing in order to shorten the name of my directory and cd into it.

## My Solve
**Flag:** `pwn.college{4FZklwVUE1AUkgC_-UJ-waOiCzk.QXxIDO0wiN0EzNzEzW}`

In the problem statement, it was provided that, by using the * argument with my command , I can get the flag.
```
hacker@globbing~matching-with-:/challenge$ /challenge/run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{4FZklwVUE1AUkgC_-UJ-waOiCzk.QXxIDO0wiN0EzNzEzW}

```

## What I learned
When it encounters a * character in any argument, the shell will treat it as a "wildcard" and try to replace that argument with any files that match the pattern.

## References
The problem statement was the reference used.
```
Now, practice this yourself! Starting from your home directory, change your directory to /challenge, but use globbing to keep the argument you pass to cd to at most four characters! Once you're there, run /challenge/run for the flag!
```

# 2. Matching with ?
The challenge prompted me to know more about ? arguments and how they work with different commands.

## My solve
**Flag:** `pwn.college{EaU-lXpQGk9brHd-3xLUbo0AToA.QXyIDO0wiN0EzNzEzW}`

I was provided in the problem statement that ? argument can help me get the flag.

```
hacker@globbing~matching-with-:~$ cd /?ha??enge
hacker@globbing~matching-with-:/challenge$ /challenge/run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{EaU-lXpQGk9brHd-3xLUbo0AToA.QXyIDO0wiN0EzNzEzW}
```

## What I learned

When it encounters a ? character in any argument, the shell will treat it as a single-character wildcard. This works like *, but only matches one character.


## References
The problem statement provided was used as the reference
```
Now, practice this yourself! Starting from your home directory, change your directory to /challenge, but use the ? character instead of c and l in the argument to cd! Once you're there, run /challenge/run for the flag!
```

# 3. Matching with []
The challenge prompted me to use the [] command.

## My solve
**Flag:** `pwn.college{M914BIvz-NDmHUjXZRrxDpuK30e.QXzIDO0wiN0EzNzEzW}`

I was provided in the problem statement that by using [] command I could get the flag.

```
hacker@globbing~matching-with-:/challenge/files$ /challenge/run file_[absh]
You got it! Here is your flag!
pwn.college{M914BIvz-NDmHUjXZRrxDpuK30e.QXzIDO0wiN0EzNzEzW}
```

## What I learned
The square brackets are, essentially, a limited form of ?, in that instead of matching any character, [] is a wildcard for some subset of potential characters, specified within the brackets.

## References
The problem statement provided was used as the reference
```
hacker@dojo:~$ touch file_a
hacker@dojo:~$ touch file_b
hacker@dojo:~$ touch file_c
hacker@dojo:~$ ls
file_a	file_b	file_c
hacker@dojo:~$ echo Look: file_[ab]
Look: file_a file_b
Try it here! We've placed a bunch of files in /challenge/files. Change your working directory to /challenge/files and run /challenge/run with a single argument that bracket-globs into file_b, file_a, file_s, and file_h!
```

# 4. Matching paths with []
The challenge prompted me to use the [] command and search for the flag.

## My solve
**Flag:** `pwn.college{QP0iTIMDBDnKs2sie15BBt2E7wJ.QX0IDO0wiN0EzNzEzW}`

I was provided in the problem statement that by using [] command , I can search for the flag.

```
hacker@globbing~matching-paths-with-:~$ /challenge/run /challenge/files/file_[absh]
You got it! Here is your flag!
pwn.college{QP0iTIMDBDnKs2sie15BBt2E7wJ.QX0IDO0wiN0EzNzEzW}
```

## What I learned
Globbing happens on a path basis, so you can expand entire paths with your globbed arguments.

## References
The problem statement provided was used as the reference
```
Now it's your turn. Once more, we've placed a bunch of files in /challenge/files. Starting from your home directory, run /challenge/run with a single argument that bracket-globs into the absolute paths to the file_b, file_a, file_s, and file_h files!

```

# 5. Multiple Globs
The challenge prompted me to have multiple globs in a single word.

## My solve
**Flag:** `pwn.college{A6PAJ4UDHr-ZtXEXcpnAyGegOZI.0lM3kjNxwiN0EzNzEzW}`

I was provided in the problem statement that by using glob commands , I can create multiple globs and find the flag.

```
hacker@globbing~multiple-globs:/challenge/files$ /challenge/run *p*
You got it! Here is your flag!
pwn.college{A6PAJ4UDHr-ZtXEXcpnAyGegOZI.0lM3kjNxwiN0EzNzEzW}
```

## What I learned
The shell looks for all files in / that start with anything (including nothing), then have an f and an l, and end in anything (including ag, which makes flag).

## References
The problem statement provided was used as the reference
```
Now you try it. We put a few happy, but diversely-named files in /challenge/files. Go cd there and run /challenge/run, providing a single argument: a short (3 characters or less) globbed word with two * globs in it that covers every word that contains the letter p.

```

# 6. Mixing globs
The challenge prompted me to use all my knowledge of globbing and find the flag.

## My solve
**Flag:** `pwn.college{kQFWZ4S5Y6UjJ2cVq5Yq8ml8kyf.QX1IDO0wiN0EzNzEzW}`

I was provided in the problem statement that by using glob commands, I can get the flag.

```
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run [cpe]*
You got it! Here is your flag!
pwn.college{kQFWZ4S5Y6UjJ2cVq5Yq8ml8kyf.QX1IDO0wiN0EzNzEzW}


```

## What I learned
Globbing can be very helpful for find data.

## References
The problem statement provided was used as the reference
```
Now, let's put the previous levels together! We put a few happy, but diversely-named files in /challenge/files. Go cd there and, using the globbing you've learned, write a single, short (6 characters or less) glob that (when passed as an argument to /challenge/run) will match the files "challenging", "educational", and "pwning"!

```

# 7. Exclusionary Globbing
The challenge prompted me to filter out files in glob using inverting.

## My solve
**Flag:** `pwn.college{00XD4OIwvjkqGaINL02DfvUIsj2.QX2IDO0wiN0EzNzEzW}`

I was provided in the problem statement that by using [!] , i can invet and filter out files to get the flag.

```
hacker@globbing~exclusionary-globbing:/challenge/files$ /challenge/run [!pwn]*
You got it! Here is your flag!
pwn.college{00XD4OIwvjkqGaINL02DfvUIsj2.QX2IDO0wiN0EzNzEzW}

```

## What I learned
 [] helps you do just this. If the first character in the brackets is a ! or (in newer versions of bash) a ^, the glob inverts, and that bracket instance matches characters that aren't listed.

## References
The problem statement provided was used as the reference
```
Armed with this knowledge, go forth to /challenge/files and run /challenge/run with all files that don't start with p, w, or n!

NOTE: The ! character has a different special meaning in bash when it's not the first character of a [] glob, so keep that in mind if things stop making sense! ^ does not have this problem, but is also not compatible with older shells.
```

# 8. Tab Completion
The challenge prompted me to use tab completion in order to auto complete my command.

## My solve
**Flag:** `pwn.college{gMKK7X77zbD5tweGZLu9oI6Mlke.0FN0EzNxwiN0EzNzEzW}`

I was provided in the problem statement that by tab complete , I can find my flag.

```
hacker@globbing~tab-completion:~$ cat /challenge/pwncollege​ 
pwn.college{gMKK7X77zbD5tweGZLu9oI6Mlke.0FN0EzNxwiN0EzNzEzW}

```

## What I learned
A safer alternative when you are trying to specify a specific target is tab completion. If you hit tab in the shell, it'll try to figure out what you're going to type and automatically complete it

When you hit that tab key, the name will expand and you'll be able to read the file.

## References
The problem statement provided was used as the reference
```
This challenge has copied the flag into /challenge/pwncollege, and you can freely cat that file. But you can't type the filename: we used some serious trickery to make sure that you must tab-complete it. Try it out!
```
# 9. Multiple options for Tab Completion
The challenge prompted me to use tab completion in order to auto complete my command when there are multiple alternatives for the command.

## My solve
**Flag:** `pwn.college{Yil-vzcOhUeleT7mWydSns16cKZ.0lN0EzNxwiN0EzNzEzW}`

I was provided in the problem statement that by tab complete , I can find my flag.

```
hacker@globbing~multiple-options-for-tab-completion:~$ cat /challenge/files/pwncollege-flag
pwn.college{Yil-vzcOhUeleT7mWydSns16cKZ.0lN0EzNxwiN0EzNzEzW}

```

## What I learned

When you hit that tab key, the name will expand and you'll be able to read the file.

 By default bash will auto-expand until the first point when there are multiple options (in this case, fl). When you hit tab a second time, it'll print out those options. Other shells and configurations, instead, will cycle through the options.

## References
The problem statement provided was used as the reference
```
This challenge has a /challenge/files directory with a bunch of files starting with pwncollege. Tab-complete from /challenge/files/p or so, and make your way to the flag!
```
# 10. Tab completion on commands
The challenge prompted me to use tab completion in order to auto complete my command.

## My solve
**Flag:** `pwn.college{wGlFe8jOjeFJ9hlg-NXflHJnAYw.0VN0EzNxwiN0EzNzEzW}`

I was provided in the problem statement that by tab complete , I can find my flag.

```
hacker@globbing~tab-completion-on-commands:~$ pwncollege-23442 
Correct! Here is your flag:
pwn.college{wGlFe8jOjeFJ9hlg-NXflHJnAYw.0VN0EzNxwiN0EzNzEzW}

```

## What I learned

When you hit that tab key, the name will expand and you'll be able to read the file.

 By default bash will auto-expand until the first point when there are multiple options (in this case, fl). When you hit tab a second time, it'll print out those options. Other shells and configurations, instead, will cycle through the options.

## References
The problem statement provided was used as the reference
```
NOTE: You can auto-complete any command, but be careful: callous auto-completes without double-checking the result can wreak havoc in your shell if you accidentally run the wrong commands!
```
