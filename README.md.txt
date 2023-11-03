GitHub is a web-based app that lets you host files in repositories, collaborate on work, and track changes to files over time. Version tracking on GitHub is powered by the open source software Git. Whenever you update a repository on GitHub, Git tracks the changes you make.
A remote URL is Git's fancy way of saying "the place where your code is stored." That URL could be your repository on GitHub, or another user's fork, or even on a completely different server.

You can only push to two types of URL addresses:

An HTTPS URL like https://github.com/user/repo.git
An SSH URL, like git@github.com:user/repo.git
Git associates a remote URL with a name, and your default remote is usually called origin.

Creating remote repositories
You can use the git remote add command to match a remote URL with a name. For example, you'd type the following in the command line:

git remote add origin <REMOTE_URL>
This associates the name origin with the REMOTE_URL.

You can use the command git remote set-url to change a remote's URL.

Adding a remote repository
To add a new remote, use the git remote add command on the terminal, in the directory your repository is stored at.

The git remote add command takes two arguments:

A remote name, for example, origin
A remote URL, for example, https://github.com/OWNER/REPOSITORY.git
For example:

$ git remote add origin https://github.com/OWNER/REPOSITORY.git
# Set a new remote

$ git remote -v
# Verify new remote
> origin  https://github.com/OWNER/REPOSITORY.git (fetch)
> origin  https://github.com/OWNER/REPOSITORY.git (push)