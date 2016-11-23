# Make Python Repo

This is a simple shell script for initializing a new Python repo on GitHub.  

### Installing

Once cloned, run

`chmod +x make-python-repo`

to make the file executable.  Then, run

`sudo cp ./make-python-repo /usr/bin`

Now the command should be executable from the prompt.

### Usage

Once installed it can be executed on the prompt with the command `make-python-repo`.

It'll then prompt you for your GitHub details, including an API token.  If you don't have one to hand, you can create a new one from https://github.com/settings/tokens.  Note that while GitHub will display your key immediately after creation, it won't display it again so you may want to make a (secure) note of it somewhere.

Based on your inputs the script will create and initialize a local repo (in a subdirectory of the path you execute it in).  It'll pull a Python/JetBrains .gitignore file and a README.md template, then create a matching repository in your GitHub account before adding it as upstream and pushing the files to it.
