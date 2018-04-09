# Managing installations on braid

### Conda is awesome
you can learn all about it from their [great documentation](https://conda.io/docs/) 
This page is meant to just be a quick and dirty cheat sheet for ideas about using it on our servers

### I have time for nothing, just gimme the path
Start by editing your bashrc file.  This is a hidden file in your home directory.  You can read it like this:
`less ~/.bashrc` or edit it using `nano ~/.bashrc`

In your bashrc file you can just add the path to where Lizzy has a directory of files installed, 
the line in your path should look like this:
`export PATH=$PATH:/home/ewilbanks/software/anaconda2/bin`

This might get you most things quickly, but...
1. you can't install things super easily
2. you can't "contain" your different programs so they don't interfere
3. you're at the whim of what Lizzy changes in this directory (yikes)

### Getting your OWN set up
1. Download and install Anaconda (lots of packages included) or miniconda (more barebone): [see here](https://docs.anaconda.com/anaconda/install/linux.html)
2. Run through start up and intro materials (here)[https://conda.io/docs/user-guide/getting-started.html]
3. Set up BioConda as a channel: follow directions (here)[https://bioconda.github.io/]
4. INSTALL ALL THE THINGS! :tada:
