# Git For Noobs

![Git Picture](https://cdn-images-1.medium.com/fit/t/1600/480/1*S-_fv45WT4MgqtnPVsxtHQ.jpeg)

The more you evolve in the world of technology, the more you will hear about 'repository' or 'deposit' or 'git' or 'hub'_, in short terms that seem to come from another dimension, but which, believe me are extremely simple.
First of all, it is necessary to make the difference in *git* and the other ennumerated ones; indeed, they work so synchro, and are so used together that one would let it be believed that it is the same thing.

## What is git

Git is what is called a _version controller_ in simple version controller of all the files in a project. No matter the type of project, no matter what type of files.

* What is _version controller_?

     Well we can say that when you evolve in your projects you create files, you delete others, you modify the contents of some and you rename certain files; git can allow you to keep track ogf this evolution as you move forward in your work; that is to say, all the changes you make allows you not only to save them, but also to return to them even after several days, without having to delete anything, because it keeps each version of each file.

### What is a deposit

First of all you have to know that his name differs (hub, repos ...), but they mean the same thing.
A repository is a remote server allowing to save your projects as well as graphically manage the versions of your files and make modifications on some files, go back, re-download the project ... because git all alone without repos always stays locally, that is to say on your machine, hence the importance of using a repos (or deposit that means the same thing)
And more importantly, putting your project on a repository allows you to work with a team on your project
There are several repositories but the best known are [Github](https://github.com/), [BitBucket](https://bitbucket.org/), [Gitlab](https://gitlab.com/) ...

#### How to use git

Install git, and open your command line.
As simple as that.
Now in practical using it consits to write in your command line git then an order. So we will have:
Once in your project from the command line, you will first initialize the git environment to tell him 'hey! manage me my project please ^ _ ^' and it is done with the command

* git init

    Once done, you have the environment on your project and you can start working.

By doing a

* git status

    You can see all the interactions that you had with the different files of your project (files modified, deleted, renamed, added ...)

But so far, git has not yet taken into account everything you just did, and that's normal because he's waiting for you to tell him that and that's why when you do a _git status_ you see in red.
So that git take them into account you will have to do

* git add .

    The '.' means all the files, but sometimes you will not want to take everything, but just a file, and you can just do:
    git add file_name

After that, redo a _git status_ you will see that the files added to the git support will be green.
Now you can initialize a project with git, see your changes and add files to git support (Hooray !!)

HOWEVER you have not yet said how to save what you did. It's very simple too, you just do

* git commit

    This command comes with options, the one you need to know is the -m which allows you among others to name your backup that will be called version as it will find you more easily when searching on different versions ( backups). So:
    git commit -m "Name of backup"

Now as said above even if you have the history of the evolution of your work on each file well organized and everything, your project is always on your machine and the changes are visible only by you.
To put your project on a remote server (here a repos) you go on a:

* [Github](https://github.com/) (conseil)
* [BitBucket](https://bitbucket.org/)
* [Gitlab](https://gitlab.com/)
* ...

Basically they all work the same way.
You create an account if you do not have one already (it's free for the life well it is not necessary to use some options anyways you do not need them -_-)
And then you click on create a repos then the steps are very easy to follow (preferably put the name of the rest, scrolls down and click on create the rest we will talk about it again)

Once done you will see clone or download somewhere on the screen (on github it's on your right)
Click on it and copy the link
Now come back to your command line (still being on your project) and put the following command

* git remote add origin link_copied

    In short, this command means that from now on, each time you make a modification on your project, you send it to the repository that is on this link

And to send the changes on the deposit you just have to do just

* git push

    At first it can tell you that you must first type another command, and that's normal this is the first time you send the content of the project you're on, copies just the command that git gave and press enter

Very important too, if we work with others, to recover the changes that a member of your team has just made

* git pull

    git will first test if there have been any changes to the projects you do not have yet, and if so, it will create a savepoint (version) and then update your project

That's ^ _ ^
