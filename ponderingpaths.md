# Challenge 1 The Root

Alright, so the filesystem starts at /. Under that, there are a whole mess of other directories, configuration files, programs, and, most importantly, flags. In this level, we've added a program right in /, called pwn, that will give you the flag. All you need to do for this level is to invoke this program!

You can invoke a program by providing its path on the command line. In this case, you'll be giving the exact path, starting from /, so the path would be /pwn. This style of path, one that starts with the root directory, is referred to as an "absolute path".

Start the challenge, launch a terminal, invoke the pwn program using its absolute path, and Capture that Flag! Good luck!

## Solution:

Since we have to write absolute path and invoke pwn.We will start from / as it denotes the root directory then directly write pwn as pwn is present right in /.


Use this blob for pasting commands you've run
```sh
hacker@paths~the-root:~$ /pwn
BOOM!!!
Here is your flag:
pwn.college{Eux-VoY2j9KBFwvhj14CNFGFn4w.QX4cTO0wCM2AzNzEzW}
```

## Flag: 

```
pwn.college{ Eux-VoY2j9KBFwvhj14CNFGFn4w.QX4cTO0wCM2AzNzEzW}
```


### References:

- [link 1](https://pwn.college)
- 
### Notes:

The root of the filesystem is a directory written as /.You refer to files and directories by their path.
A path from the root of the filesystem starts with / (that is, the root of the filesystem)

