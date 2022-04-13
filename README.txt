here a summury to my journey with git and github:
git is a an open source software for code versioning and tracking, it gives the ability to many devs to work on the same 
projects by monitoring and keeping history of all changes done to the code;
to jumb in first need to install git on ur machine,sometimes it comes by default installed,check it with comand:git --version
otherwise you need to install it.after a wise thing to do is running a help command to have an idea about it:
run git --help.
now we go with with github, its a web based location where people store their repositories , they can work directy on it their online,
or better to dowload it to their local machine(clone),change or (add) files ,saving your changes(commit),and than uploading back to github(push).
here we listed few commands to start with,and to have an idea what git is for.

next to do all this ,a configuration is needed to make all working perfect:
personalize ur git account with name and email,and editor you use like vscode ,:

git config --global user.name "youname"
git config --global user.email "youremail"
git config --global core.editor "editor u use" 

there are other advanced options to config, finally you can check your configuration by running:
git config --list
now we have to figure out how to connect from your local machine to github ;with 2 ways :
running git commnad followed by your git repository URL,logging prompt will ask you your email and psw,but recently this method was abandoned for a tekonized log in ,see github guide.
other simplest and efficient  way is to ssh from your machine to github:
we need to generate a ssh keys with option -C "email used to log in github" in on local machine:
run ssh key-gen -t 56678 -C "email"
this will generate a file with 2 keys, a private and a public one,,you need to copy the public one in your github account setting regarding ssh .
and your are done
now we try changes to add some lines to this files and trying to push it again 
