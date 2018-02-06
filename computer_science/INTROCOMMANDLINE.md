# Intro to the Command line

This page is here to lessen the learning curve for new ACM members who have never used a 
commandline. Currently this contains only a guide for `bash` (Bourne Again Shell).

## Anatomy of the Terminal

Start out by launching a terminal, it will look like this.

    [username@localmachine ~ ] $ 

you should see your username name before the @ symbol.
 This is followed by the name of your computer. The ~ means that the terminal is currently looking at your
home directory. This is where you will input commands.

### <span style="color:red">**Warning!!!**</span>

 If you see the username `root` it means that you are running the terminal as a very powerful user named 
 `root`. `root` has ultimate privaliges on your machine and might as well be god as far as your computer is 
 conserned. With great power comes great responcibility and running as `root` is considered very dangerous 
 because you can easily destroy your operating system. To switch out of `root` type:

    $ su yourUserName

## Useful Commands

    $ cd directory/
This lets you change the directory that you are in. This is how you will navigate your computer.

    $ ls
This will show you every file and directory in you current working directory (the current working directory is displayed where that ~ was when you first loaded up the terminal).

    $ pwd
This is short for "print working directory." This will show where your terminal is looking at.

    $ man <command>
This brings up the manual page for whatever comand you specify. This will be your best friend!

## <span style="color:yellow">Don't Panic</span>
There is a lot to learn when it comes to learning the comand line, and you will not be expected to learn everything all at once. You are also not alone, feel free to ask other ACM members  for help. Included below are some places where you can learn more.

- Linuxcommand.org 
    - This is a good place to start, and will teach you everything from your first command to making `bash` scripts.
- More is to come in the future

