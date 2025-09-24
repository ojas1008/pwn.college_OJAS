# 1. The Roots
The challenge prompted me to invoke a program by providing its path on the command line.

## My Solve
**Flag:** `pwn.college{Eux-VoY2j9KBFwvhj14CNFGFn4w.QX4cTO0wCM2AzNzEzW}`

In the problem statement, it was provided that, the ' / ' command and invoking a program would provide the flag.
```
hacker@paths~the-root:~$ /pwn
BOOM!!!
Here is your flag:
pwn.college{Eux-VoY2j9KBFwvhj14CNFGFn4w.QX4cTO0wCM2AzNzEzW}
```

## What I learned
I learnt to invoke a program by providing its path on the command line,
In this case, I gave the exact path, starting from /, so the path would be /pwn. This style of path, one that starts with the root directory, is referred to as an "absolute path".

## References
The problem statement was the reference used.
```


You can invoke a program by providing its path on the command line. In this case, you'll be giving the exact path, starting from /, so the path would be /pwn. This style of path, one that starts with the root directory, is referred to as an "absolute path".

Start the challenge, launch a terminal, invoke the pwn program using its absolute path, and Capture that Flag! Good luck!
```

# 2. Program and Absolute Paths
The challenge prompted me invoke a program using its absolute path.

## My solve
**Flag:** `pwn.college{YP0sGFIwXLwK8Rn03lLc4srHQ77.QX1QTN0wCM2AzNzEzW}`

I was provided in the problem statement that using /challenge/run , I can find the run program which holds the flag.

```
hacker@paths~program-and-absolute-paths:~$ /challenge/run
Correct!!!
/challenge/run is an absolute path! Here is your flag:
pwn.college{YP0sGFIwXLwK8Rn03lLc4srHQ77.QX1QTN0wCM2AzNzEzW}
```

## What I learned
I learnt that challenges in pwn.college are in the challenge directory and the challenge directory is, in turn, right in the root directory (/). The path to the challenge directory is, thus, /challenge. The name of the challenge program in this level is run, and it lives in the /challenge directory. Thus, the path to the run challenge program is /challenge/run.

## References
The problem statement provided was used as the reference
```
Let's explore a slightly more complicated path! Except for in the previous level, challenges in pwn.college are in the challenge directory and the challenge directory is, in turn, right in the root directory (/). The path to the challenge directory is, thus, /challenge. The name of the challenge program in this level is run, and it lives in the /challenge directory. Thus, the path to the run challenge program is /challenge/run.
This challenge again requires you to execute it by invoking its absolute path. You'll want to execute the run file that is in the challenge directory that is, in turn, in the / directory. If you invoke the challenge correctly, it will give you the flag. Good luck!
```

# 3. Position thy self
The challenge prompted me to navigate around directories to find my desired program.

## My solve
**Flag:** `pwn.college{s_J0K5A5jqyCPBZPRqdnaMm5fEC.QX2QTN0wCM2AzNzEzW}`

I was provided in the problem statement that by using cd command , I can find the my desired program which holds the flag.

```
hacker@paths~position-thy-self:~$ /challenge/run
Incorrect...
You are not currently in the /var/lib/apt/lists directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-thy-self:/sys$ cd /var/lib/apt/lists
hacker@paths~position-thy-self:/var/lib/apt/lists$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{s_J0K5A5jqyCPBZPRqdnaMm5fEC.QX2QTN0wCM2AzNzEzW}
```

## What I learned
cd command means change directory , which can navigate user around directories. I found out the path's directory and then found /challenge/run program in thaat directory specified.

## References
The problem statement provided was used as the reference
```
The Linux filesystem has tons of directories with tons of files. You can navigate around directories by using the cd (change directory) command and passing a path to it as an argument, as so:

hacker@dojo:~$ cd /some/new/directory
hacker@dojo:/some/new/directory$
This affects the "current working directory" of your process (in this case, the bash shell). Each process has a directory in which it's currently hanging out. The reasons for this will become clear later in the module.

As an aside, now you can see what the ~ was in the prompt! It shows the current path that your shell is located at.

This challenge will require you to execute the /challenge/run program from a specific path (which it will tell you). You'll need to cd to that directory before rerunning the challenge program. Good luck!
```

# 4. Position elsewhere
The challenge prompted me to navigate around directories to find my desired program.

## My solve
**Flag:** `pwn.college{wCb6qsV6QPr2Hq0ZdCpKPqkhVWo.QX3QTN0wCM2AzNzEzW}`

I was provided in the problem statement that by using cd command , I can find the my desired program which holds the flag.

```
hacker@paths~position-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /proc/131/fd directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-elsewhere:~$ cd /proc/131/fd
hacker@paths~position-elsewhere:/proc/131/fd$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{wCb6qsV6QPr2Hq0ZdCpKPqkhVWo.QX3QTN0wCM2AzNzEzW}
```

## What I learned
cd command means change directory , which can navigate user around directories. I found out the path's directory and then found /challenge/run program in thaat directory specified.

## References
The problem statement provided was used as the reference
```
The Linux filesystem has tons of directories with tons of files. You can navigate around directories by using the cd (change directory) command and passing a path to it as an argument, as so:

hacker@dojo:~$ cd /some/new/directory
hacker@dojo:/some/new/directory$
This affects the "current working directory" of your process (in this case, the bash shell). Each process has a directory in which it's currently hanging out. The reasons for this will become clear later in the module.

As an aside, now you can see what the ~ was in the prompt! It shows the current path that your shell is located at.

This challenge will require you to execute the /challenge/run program from a specific path (which it will tell you). You'll need to cd to that directory before rerunning the challenge program. Good luck!


```

# 5. Position yet elsewhere
The challenge prompted me to navigate around directories to find my desired program.

## My solve
**Flag:** `pwn.college{otFZffpuIgtUiLBZh7lcdbeb8Sz.QX4QTN0wCM2AzNzEzW}`

I was provided in the problem statement that by using cd command , I can find the my desired program which holds the flag.

```
hacker@paths~position-yet-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /etc directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-yet-elsewhere:~$ cd /etc
hacker@paths~position-yet-elsewhere:/etc$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{otFZffpuIgtUiLBZh7lcdbeb8Sz.QX4QTN0wCM2AzNzEzW}
```

## What I learned
cd command means change directory , which can navigate user around directories. I found out the path's directory and then found /challenge/run program in thaat directory specified.

## References
The problem statement provided was used as the reference
```
The Linux filesystem has tons of directories with tons of files. You can navigate around directories by using the cd (change directory) command and passing a path to it as an argument, as so:

hacker@dojo:~$ cd /some/new/directory
hacker@dojo:/some/new/directory$
This affects the "current working directory" of your process (in this case, the bash shell). Each process has a directory in which it's currently hanging out. The reasons for this will become clear later in the module.

As an aside, now you can see what the ~ was in the prompt! It shows the current path that your shell is located at.

This challenge will require you to execute the /challenge/run program from a specific path (which it will tell you). You'll need to cd to that directory before rerunning the challenge program. Good luck!


```

# 6. implicit relative paths, from /
The challenge prompted me to navigate around directories using relative paths in order to find my desired program.

## My solve
**Flag:** `pwn.college{kli88PmRdVwwN080YwG4qSD9-kq.QX5QTN0wCM2AzNzEzW}`

I was provided in the problem statement that by using relative paths  , I can find the my desired program which holds the flag.

```
hacker@paths~implicit-relative-paths-from-:~$ /challenge/run
Incorrect...
You are not currently in the / directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~implicit-relative-paths-from-:~$ cd /
hacker@paths~implicit-relative-paths-from-:/$ challenge/run
Correct!!!
challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{kli88PmRdVwwN080YwG4qSD9-kq.QX5QTN0wCM2AzNzEzW}



```

## What I learned
A relative path is any path that does not start at root (i.e., it does not start with /).
A relative path is interpreted relative to ones current working directory (cwd).
cwd is the directory that my prompt is currently located at.

## References
The problem statement provided was used as the reference
```
However, the current working directory does matter for relative paths.

A relative path is any path that does not start at root (i.e., it does not start with /).
A relative path is interpreted relative to your current working directory (cwd).
Your cwd is the directory that your prompt is currently located at.
This means how you specify a particular file, depends on where the terminal prompt is located.

Imagine we want to access some file located at /tmp/a/b/my_file.

If my cwd is /, then a relative path to the file is tmp/a/b/my_file.
If my cwd is /tmp, then a relative path to the file is a/b/my_file.
If my cwd is /tmp/a/b/c, then a relative path to the file is ../my_file. The .. refers to the parent directory.
Let's try it here! You'll need to run /challenge/run using a relative path while having a current working directory of /.

```

# 7. explicit relative paths, from /
The challenge prompted me to navigate around directories using explicit relative paths in order to find my desired program.

## My solve
**Flag:** `pwn.college{MfmyGdOZ6xEKguq3Df9WRuNgvpE.QXwUTN0wCM2AzNzEzW}`

I was provided in the problem statement that by using explicit relative paths  , I can find the my desired program which holds the flag.

```
hacker@paths~explicit-relative-paths-from-:~$ cd /
hacker@paths~explicit-relative-paths-from-:/$ ./challenge/ru
n
Correct!!!
./challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{MfmyGdOZ6xEKguq3Df9WRuNgvpE.QXwUTN0wCM2AzNzEzW}



```

## What I learned
I learnt that the following relative paths are all identical to each other:

challenge
./challenge
./././challenge
challenge/.

## References
The problem statement provided was used as the reference
```
In most operating systems, including Linux, every directory has two implicit entries that you can reference in paths: . and ... The first, ., refers right to the same directory, so the following absolute paths are all identical to each other:

/challenge
/challenge/.
/challenge/./././././././././
/./././challenge/././
The following relative paths are also all identical to each other:

challenge
./challenge
./././challenge
challenge/.
Of course, if your current working directory is /, the above relative paths are equivalent to the above absolute paths.

This challenge will get you using . in your relative paths. Get ready!

```

# 8. implicit relative path
The challenge prompted me to navigate around directories using explicit relative paths in order to find my desired program.

## My solve
**Flag:** `pwn.college{UJPW5v1IU7z-8y3wjXd_pdDaCxc.QXxUTN0wCM2AzNzEzW}`

I was provided in the problem statement that by using explicit relative paths  , I can find the my desired program which holds the flag.

```
hacker@paths~implicit-relative-path:~$ cd /challenge
hacker@paths~implicit-relative-path:/challenge$ ./run
Correct!!!
./run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{UJPW5v1IU7z-8y3wjXd_pdDaCxc.QXxUTN0wCM2AzNzEzW}

```

## What I learned
I learnt that the following relative paths are all identical to each other:

challenge
./challenge
./././challenge
challenge/.

## References
The problem statement provided was used as the reference
```
Linux explicitly avoids automatically looking in the current directory when you provide a "naked" path. Consider the following:

hacker@dojo:~$ cd /challenge
hacker@dojo:/challenge$ run
This will not invoke /challenge/run. This is actually a safety measure: if Linux searched the current directory for programs every time you entered a naked path, you could accidentally execute programs in your current directory that happened to have the same names as core system utilities!

```

# 9. home sweet home
The challenge prompted me to navigate around directories by creating my own path name in home in order to find desired flag.

## My solve
**Flag:** `pwn.college{0_YZm-5u5eq2J1SXI4sX7PQpmKz.QXzMDO0wCM2AzNzEzW}`

I was provided in the problem statement that by using absolute path in home , I can find the my desired program which holds the flag.

```
hacker@paths~home-sweet-home:~$ /challenge/run ~/.a
The argument you provided must not have been longer than 3 characters (it's
currently 4 characters long)!
hacker@paths~home-sweet-home:~$ /challenge/run ~/a
Writing the file to /home/hacker/a!
... and reading it back to you:
pwn.college{0_YZm-5u5eq2J1SXI4sX7PQpmKz.QXzMDO0wCM2AzNzEzW}

```

## What I learned
Note that the expansion of ~ is an absolute path, and only the leading ~ is expanded. This means, for example, that ~/~ will be expanded to /home/hacker/~ rather than /home/hacker/home/hacker.

## References
The problem statement provided was used as the reference
```
Fun fact: cd will use your home directory as the default destination:

hacker@dojo:~$ cd /tmp
hacker@dojo:/tmp$ cd
hacker@dojo:~$
Now it's your turn to play! In this challenge, /challenge/run will write a copy of the flag to any file you specify as an argument on the commandline, with these constraints:

Your argument must be an absolute path.
The path must be inside your home directory.
Before expansion, your argument must be three characters or less.
```
