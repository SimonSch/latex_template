# Git & Latex Template

## Installation

### Windows

* [Git download](https://git-scm.com/download/win)
* [Tex studio](https://www.texstudio.org/) ~ latex editor
* [Miktex](https://miktex.org/) ~ latex compiler

### Linux 

```
sudo apt-get install git
```
 

```
sudo apt-get install texlive 
sudo apt-get install texlive-lang-<YOUR_LANG> eg. install texlive-lang-german

I have no idea what Im doing... 
sudo apt-get install texlive-full

```

```
sudo apt-get install texstudio
```

#####  Linux Config
Add the following to ~./bashrc to display the current branch
```bash
# show git branch name
force_color_prompt=yes
color_prompt=yes
parse_git_branch() {
         git branch 2> /dev/null | sed -e '/^[^*]/d' -e 's/* \(.*\)/(\1)/'
 }
 if [ "$color_prompt" = yes ]; then
          PS1='${debian_chroot:+($debian_chroot)}\[\033[01;32m\]\u@\h\[\033[00m\]:\[\033[0$
  else
           PS1='${debian_chroot:+($debian_chroot)}\u@\h:\w$(parse_git_branch)\$ '
   fi
unset color_prompt force_color_prompt

```

## Git Services

* [Github](https://github.com/)
* [Bitbucket](https://bitbucket.org/)

## TL;DR
* git clone https://your-repository.com
* add files 
* git status
* git add "files.bla"
* git status
* git commit -m "Your commit message" 
* git config --global user.email "you@example.com" 
* git config --global user.name "Your Name"
* git push 

## Git Cheatsheet 

![git](./git-cheat-sheet-large01.png?raw=true)
