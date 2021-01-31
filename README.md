# Using `git`
This is an introductory repository designed to help understand how the version control program `git` works and how it can help make collaborating and working on projects easier.

For easier viewing, an [html version](https://htmlpreview.github.io/?https://github.com/utkuboduroglu/using-git-test/blob/master/README.html) of the README is also available.

## Why use git?
For any sort of project -- not necessarily just programming -- a version control program helps keep track of what changes were made to the project. Such programs eliminate the need to manually backup projects, and allows you to see previous versions of your project. Because of this, git is a really popular choice to maintain a project.

## How it works
Very simply, git keeps track of your edits in a graph. You can check out nodes of this graph to view the previous edits on the project, or commit new nodes to add new changes. These graphs can then be synchronized to cloud services, like Github or BitBucket.

## How do I use `git`?
We will go over the terminal version of git in this tutorial, although you can do everything mentioned here over in a GUI version of git as well.

If you get lost at any step, you can always check out `git --help` to see a help page provided by the program itself.

### Initializing our repository
In order to use git, we need to tell it that we intend to use a directory as a project. We use the command **git init** to tell git that we have a project in our current directory:

<pre>
$ <kbd>git init</kbd>
Initialized empty Git repository in .../project/.git/
</pre>

When we run the command, we see the prompt above telling us that we created a git repo in the `project/` directory.

### Cloning an already existing repository
If the project you're going to be working on already exists, you can instead 'clone' that project onto your machine. For example, let's say that you wanted to clone this repository onto your machine. To do this, you would use the clone command of git, and specify a path (either local or online) to a git repository to clone it:

<pre>
$ <kbd>git clone https://github.com/utkuboduroglu/using-git-test</kbd>
Cloning into 'using-git-test'...
remote: Enumerating objects: 4, done.
remote: Counting objects: 100% (4/4), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 4 (delta 1), reused 4 (delta 1), pack-reused 0
Receiving objects: 100% (4/4), done.
Resolving deltas: 100% (1/1), done.
</pre>

Although your prompt may not look exactly the same, this is the output you would get, showing where you cloned the project to, and how many objects you cloned. As an exercise, **try cloning this repository onto your machine.** We will use this repository as an example of how a git workflow works.

### Adding changes
After you either created or cloned your repository, you may want to make some edits and tell git to keep track of those edits. For example, open this `README.md` file in a text editor and change the line below:

<pre>
<kbd> CHANGE ME </kbd>
</pre>