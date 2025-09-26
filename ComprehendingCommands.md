# 1. cat:not the pet,but the command
The challenge prompted me to use the cat command and see how it works.

## My Solve
**Flag:** `pwn.college{0ogZKpxE1YVVo1E42r743au7fLl.QXxcTN0wCM2AzNzEzW}`

In the problem statement, it was provided that, the ' cat ' command can be used to read the flag file to get the flag.
```
hacker@commands~cat-not-the-pet-but-the-command:~$ cat /flag
pwn.college{0ogZKpxE1YVVo1E42r743au7fLl.QXxcTN0wCM2AzNzEzW}
```

## What I learned
I learnt to invoke the cat command. cat comes from the word concatenate , and it can read multiple files at a time.

## References
The problem statement was the reference used.
```

Finally, if you give no arguments at all, cat will read from the terminal input and output it. We'll explore that in later challenges...

In this challenge, I will copy the flag to the flag file in your home directory (where your shell starts). Go read it with cat!
```

# 2. catting absolute paths
The challenge prompted me invoke a cat command using its absolute path.

## My solve
**Flag:** `pwn.college{oJEdcThapUk5bohQNvAoYB7ZsK6.QX5ETO0wCM2AzNzEzW}`

I was provided in the problem statement that using cat command by absolute path , I can find the flag program which holds the flag.

```
hacker@commands~catting-absolute-paths:~$ cat /flag
pwn.college{oJEdcThapUk5bohQNvAoYB7ZsK6.QX5ETO0wCM2AzNzEzW}
```

## What I learned
I learned that cat command can also be used with absolute paths.

## References
The problem statement provided was used as the reference
```
In this directory, I will not copy it to your home directory, but I will make it readable. You can read it with cat at its absolute path: /flag.

FUN FACT: /flag is where the flag always lives in pwn.college, but unlike in this challenge, you typically can't access that file directly.
```

# 3. more catting practice
The challenge prompted me to use the cat command and see how it works.

## My Solve
**Flag:** `pwn.college{Yat4ERYQuwqBaUbz55IPl7FrcxS.QXwITO0wCM2AzNzEzW}`

In the problem statement, it was provided that, the ' cat ' command can be used to read the flag file to get the flag.
```
hacker@commands~more-catting-practice:~$ cd /flag
You used 'cd'! In this level, I don't allow you to change the working directory
--- you MUST chase pass 'cat' the absolute path of where I put it on the
filesystem (which is /usr/share/texmf/flag).
hacker@commands~more-catting-practice:~$ cat /usr/share/texmf/flag
pwn.college{Yat4ERYQuwqBaUbz55IPl7FrcxS.QXwITO0wCM2AzNzEzW}
```

## What I learned
I learnt to invoke the cat command. cat comes from the word concatenate , and it can read multiple files at a time.

## References
The problem statement was the reference used.
```
You can specify all sorts of paths as arguments to commands, and we'll practice some more with cat. In this level, I'll put the flag in some crazy directory, and I will not allow you to change directories with cd, so no cat flag for you. You must retrieve the flag by absolute path, wherever it is.
```


# 4. grepping for a needle in a haystack
The challenge prompted me to invoke the grep command to search the contents we need.

## My solve
**Flag:** `pwn.college{c5v2LudLlB0uihUll2zAge3iK2A.QX3EDO0wCM2AzNzEzW}`

I was provided in the problem statement that by using grep command , I can find my desired program which holds the flag.

```
hacker@commands~grepping-for-a-needle-in-a-haystack:~$  grep pwn  /challenge/data.txt
pwn.college{c5v2LudLlB0uihUll2zAge3iK2A.QX3EDO0wCM2AzNzEzW}
pwns
pwned
pwning
pwn
```

## What I learned
grep is used to search the file for lines containing what we need.Sometimes, the files that we might cat out are too big. Luckily, we have the grep command to search for the contents we need!

## References
The problem statement provided was used as the reference
```
hacker@dojo:~$ grep SEARCH_STRING /path/to/file
Invoked like this, grep will search the file for lines of text containing SEARCH_STRING and print them to the console.

In this challenge, I've put a hundred thousand lines of text into the /challenge/data.txt file. grep it for the flag!

```

# 5. comparing files
The challenge prompted me to find changes between similar files using diff command.

## My solve
**Flag:** `pwn.college{Uc8l9dgJ_BqedHchFpWvP0nTPMH.01MwMDOxwCM2AzNzEzW}`

I was provided in the problem statement that by using diff command , I can find my desired program which holds the flag.

```
hacker@commands~comparing-files:~$ diff /challenge/decoys_only.txt /challenge/decoys_and_real.txt
87a88
> pwn.college{Uc8l9dgJ_BqedHchFpWvP0nTPMH.01MwMDOxwCM2AzNzEzW}
```

## What I learned
diff compares two files line by line and shows you exactly what's different between them.

## References
The problem statement provided was used as the reference
```
Now for your challenge! There are two files in /challenge:

/challenge/decoys_only.txt contains 100 fake flags
/challenge/decoys_and_real.txt contains all 100 fake flags plus the one real flag
Use diff to find what's different between these files and get your flag!

```

# 6. listing files
The challenge prompted me to invoke the ls command to find my desired file by listing all contents.

## My solve
**Flag:** `pwn.college{w5-GrFy2oGBokIDGcSmKNfw2lJQ.QX4IDO0wCM2AzNzEzW}`

I was provided in the problem statement that by using ls command  , I can find the my desired program which holds the flag.

```
hacker@commands~listing-files:~$ ls /challenge
20795-renamed-run-9034  DESCRIPTION.md
hacker@commands~listing-files:~$ /challenge/20795-renamed-run-9034
Yahaha, you found me! Here is your flag:
pwn.college{w5-GrFy2oGBokIDGcSmKNfw2lJQ.QX4IDO0wCM2AzNzEzW}



```

## What I learned
ls will list files in all the directories provided to it as arguments, and in the current directory if no arguments are provided. 

## References
The problem statement provided was used as the reference
```
hacker@dojo:~$ ls /challenge
run
hacker@dojo:~$ ls
Desktop    Downloads  Pictures  Templates
Documents  Music      Public    Videos
hacker@dojo:~$ ls /home/hacker
Desktop    Downloads  Pictures  Templates
Documents  Music      Public    Videos
hacker@dojo:~$
In this challenge, we've named /challenge/run with some random name! List the files in /challenge to find it.

```

# 7. touching files
The challenge prompted me to create a new file using the touch command.

## My solve
**Flag:** `pwn.college{I7NqiuG_Y2TzEkivM7mo4UEyNRI.QXwMDO0wCM2AzNzEzW}`

I was provided in the problem statement that by using touch command, I can create a new file and find the flag.

```
hacker@commands~touching-files:~$ cd /tmp
hacker@commands~touching-files:/tmp$ touch pwn
hacker@commands~touching-files:/tmp$ touch college
hacker@commands~touching-files:/tmp$ ls /tmp
bin      hsperfdata_root  tmp.4mK6TfTSUV
college  pwn
hacker@commands~touching-files:/tmp$ /challenge/run
Success! Here is your flag:
pwn.college{I7NqiuG_Y2TzEkivM7mo4UEyNRI.QXwMDO0wCM2AzNzEzW}

```

## What I learned
We can create a new, blank file by touching it with the touch command.
## References
The problem statement provided was used as the reference
```
hacker@dojo:~$ cd /tmp
hacker@dojo:/tmp$ ls
hacker@dojo:/tmp$ touch pwnfile
hacker@dojo:/tmp$ ls
pwnfile
hacker@dojo:/tmp$
It's that simple! In this level, please create two files: /tmp/pwn and /tmp/college, and run /challenge/run to get your flag!

```

# 8. removing files
The challenge prompted me use the rm command to delete files of no use.

## My solve
**Flag:** `pwn.college{gky_IdUhvom_hZaYJnomYnRm8tt.QX2kDM1wCM2AzNzEzW}`

I was provided in the problem statement that by using rm command , I can delete files and get the flag.

```
hacker@commands~removing-files:~$ rm delete_me
hacker@commands~removing-files:~$ cd /challenge
hacker@commands~removing-files:/challenge$ ls /challenge
DESCRIPTION.md  check
hacker@commands~removing-files:/challenge$ /challenge/check
Excellent removal. Here is your reward:
pwn.college{gky_IdUhvom_hZaYJnomYnRm8tt.QX2kDM1wCM2AzNzEzW}
```

## What I learned
In Linux, one removes files with the rm command.

## References
The problem statement provided was used as the reference
```
hacker@dojo:~$ touch PWN
hacker@dojo:~$ touch COLLEGE
hacker@dojo:~$ ls
COLLEGE     PWN
hacker@dojo:~$ rm PWN
hacker@dojo:~$ ls
COLLEGE
hacker@dojo:~$
Let's practice. This challenge will create a delete_me file in your home directory! Delete it, then run /challenge/check, which will make sure you've deleted it and then give you the flag!

```

# 9. moving files
The challenge prompted me to move around files using the mv command.

## My solve
**Flag:** `pwn.college{o_zzsEacKcRJ9ydH-8LWRNywm1m.0VOxEzNxwCM2AzNzEzW}`

I was provided in the problem statement that by using mv command , I can move around files and find my flag.

```
hacker@commands~moving-files:~$ mv /flag /tmp/hack-the-planet
Correct! Performing 'mv /flag /tmp/hack-the-planet'.
hacker@commands~moving-files:~$ /challenge/check
Congrats! You successfully moved the flag to /tmp/hack-the-planet! Here it is:
pwn.college{o_zzsEacKcRJ9ydH-8LWRNywm1m.0VOxEzNxwCM2AzNzEzW}
```

## What I learned
You can also move files around with the mv command.
## References
The problem statement provided was used as the reference
```
hacker@dojo:~$ ls
my-file
hacker@dojo:~$ cat my-file
PWN!
hacker@dojo:~$ mv my-file your-file
hacker@dojo:~$ ls
your-file
hacker@dojo:~$ cat your-file
PWN!
hacker@dojo:~$
This challenge wants you to move the /flag file into /tmp/hack-the-planet (do it)! When you're done, run /challenge/check, which will check things out and give the flag to you.
```

# 10. hidden files
The challenge prompted me to find hidden files by using ls -a.

## My solve
**Flag:** `pwn.college{kZUfLODRiGXfnxaYy3iOkor97Ma.QXwUDO0wCM2AzNzEzW}`

I was provided in the problem statement that by using ls -a command , I can find files that start with a ' . ' , which are generally hidden.

```
hacker@commands~hidden-files:~$ cd /
hacker@commands~hidden-files:/$ ls -a
.                     dev     media  sbin
..                    etc     mnt    srv
.dockerenv            home    nix    sys
.flag-25461189498283  lib     opt    tmp
bin                   lib32   proc   usr
boot                  lib64   root   var
challenge             libx32  run
hacker@commands~hidden-files:/$ cat /.flag-25461189498283
pwn.college{kZUfLODRiGXfnxaYy3iOkor97Ma.QXwUDO0wCM2AzNzEzW}
```

## What I learned
Interestingly, ls doesn't list all the files by default. Linux has a convention where files that start with a '.' don't show up by default in ls and in a few other contexts. To view them with ls, we need to invoke ls with the -a flag
Use cat to read that file.
## References
The problem statement provided was used as the reference
```
hacker@dojo:~$ touch pwn
hacker@dojo:~$ touch .college
hacker@dojo:~$ ls
pwn
hacker@dojo:~$ ls -a
.college	pwn
hacker@dojo:~$
Now, it's your turn! Go find the flag, hidden as a dot-prepended file in /.
```


# 11. An Epic Filesystem Quest
The challenge prompted me to use my knowledge of cd,ls and cat commands to find the flag.

## My solve
**Flag:** `pwn.college{QciMG6kNBknEpiwyliiy0V1-VT-.QX5IDO0wiN0EzNzEzW}`
I was provided in the problem statement that by using prior knowledge of different commands , I can find the flag.

```
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/Documentation/networking/caif$ cat .GIST
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{QciMG6kNBknEpiwyliiy0V1-VT-.QX5IDO0wiN0EzNzEzW}
```

## What I learned
I have to use my knowledge of ls,ls -a,cat and cd command.
## References
The problem statement provided was used as the reference
```
In this challenge, I have hidden the flag! Here, you will use ls and cat to follow my breadcrumbs and find it! Here's how it'll work:

Your first clue is in /. Head on over there.
Look around with ls. There'll be a file named HINT or CLUE or something along those lines!
cat that file to read the clue!
Depending on what the clue says, head on over to the next directory (or don't!).
Follow the clues to the flag!
Good luck!
```


# 12. making directories
The challenge prompted me to make my own directory using mkdir command.

## My solve
**Flag:** `pwn.college{g1s08RxwLtP50clPcnjOB1pVbjj.QXxMDO0wiN0EzNzEzW}`

I was provided in the problem statement that by using mkdir command , I can make my own directory and find my flag.

```
hacker@commands~making-directories:/tmp$ cd /tmp/pwn
hacker@commands~making-directories:/tmp/pwn$ touch college
hacker@commands~making-directories:/tmp/pwn$ /challenge/run
Success! Here is your flag:
pwn.college{g1s08RxwLtP50clPcnjOB1pVbjj.QXxMDO0wiN0EzNzEzW}

```

## What I learned
You make directories using the mkdir command. Then you can stick files in there!
## References
The problem statement provided was used as the reference
```
hacker@dojo:~$ cd /tmp
hacker@dojo:/tmp$ ls
hacker@dojo:/tmp$ ls
hacker@dojo:/tmp$ mkdir my_directory
hacker@dojo:/tmp$ ls
my_directory
hacker@dojo:/tmp$ cd my_directory
hacker@dojo:/tmp/my_directory$ touch my_file
hacker@dojo:/tmp/my_directory$ ls
my_file
hacker@dojo:/tmp/my_directory$ ls /tmp/my_directory/my_file
/tmp/my_directory/my_file
hacker@dojo:/tmp/my_directory$
Now, go forth and create a /tmp/pwn directory and make a college file in it!
```


# 13. finding files
The challenge prompted me to find my files using the find command.

## My solve
**Flag:** `pwn.college{Iz4k3ulbB5V35Hge1vQMgMHYSBG.QXyMDO0wiN0EzNzEzW}`

I was provided in the problem statement that by using find command , I can find my files and get my flag.

```
hacker@commands~finding-files:/$ cat ./opt/linux/linux-5.4/drivers/misc/ti-st/flag
pwn.college{Iz4k3ulbB5V35Hge1vQMgMHYSBG.QXyMDO0wiN0EzNzEzW}
```

## What I learned
The find command takes optional arguments describing the search criteria and the search location. If you don't specify a search criteria, find matches every file. If you don't specify a search location, find uses the current working directory.

## References
The problem statement provided was used as the reference
```
Now it's your turn. I've hidden the flag in a random directory on the filesystem. It's still called flag. Go find it!

Several notes. First, there are other files named flag on the filesystem. Don't panic if the first one you try doesn't have the actual flag in it. Second, there're plenty of places in the filesystem that are not accessible to a normal user. These will cause find to generate errors, but you can ignore those; we won't hide the flag there! Finally, find can take a while; be patient!
```


# 14. linking files
The challenge prompted me to establish difference between hard and soft links and how linking makes process easier on Linux.

## My solve
**Flag:** `pwn.college{0GZUMW02JO_H4B-oZWC070xMRES.QX5ETN1wiN0EzNzEzW}`

I was provided in the problem statement that by using ln -s command , I can create symlinks and find my flag.

```
hacker@commands~linking-files:~$ /challenge/catflag
About to read out the /home/hacker/not-the-flag file!
pwn.college{0GZUMW02JO_H4B-oZWC070xMRES.QX5ETN1wiN0EzNzEzW}
```

## What I learned
Links come in two flavors: hard and soft (also known as symbolic) links. We'll differentiate the two with an analogy:

A hard link is when you address your apartment using multiple addresses that all lead directly to the same place (e.g., Apt 2 vs Unit 2).

A soft link is when you move apartments and have the postal service automatically forward your mail from your old place to your new place.

Note that the original file path comes before the link path in the command!
## References
The problem statement provided was used as the reference
```
hacker@dojo:~$ file /tmp/myfile
/tmp/myfile: ASCII text
hacker@dojo:~$ file ~/ourfile
/home/hacker/ourfile: symbolic link to /tmp/myfile
hacker@dojo:~$
Okay, now you try it! In this level the flag is, as always, in /flag, but /challenge/catflag will instead read out /home/hacker/not-the-flag. Use the symlink, and fool it into giving you the flag!
```
