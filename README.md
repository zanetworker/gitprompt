# my short git prompt 

This makes your bash prompt aware of the current git branch and abbreviates the current directory to the last two directories.
Please only use this only on your local, machine or add the user/host (`\u@\h`) info to the prompt.

After installing your prompt will look something like:

```
…/parent/current (branch)$ 
```

# Installation

copy the scripts to your system bin:
  `sudo cp current-git-branch pwd-last-two /usr/local/bin`

add this to your `~/.bash_profile` on your Mac or `.bashrc` on your Linux machine:  
  `PS1="\$(pwd-last-two)\$(current-git-branch)\$ "`

or with color (only a little darker for the branch):  
  `PS1="\$(pwd-last-two)\\[\033[0;37m\]\$(current-git-branch)\[\033[0m\]\\$ "`
  
# Contribute

Please fork and pull-request me :)