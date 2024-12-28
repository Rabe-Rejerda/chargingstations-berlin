# Description
This folder cotains loosly connected utility skripts that are not used by the main program.<br>
Instead they are meant to be used by the developers to help them develop the app.

## git-hooks
The simplest way to ensure, that formats are beeing kept by all members of the team, is for everyone to use git-hooks.
#### pre-commit
The [pre-commit](./git-hooks/pre-commit) hook will execute its skript right before the commit of all added files takes place. <br>
Here the script executes the program [black](https://pypi.org/project/black/) on all given python files. Black is a code formatter that ensures that the guidelines of pep8 are kept.
#### activating the hook
To activate the hook you can use the command in a git bash environment<br>

    cd <project>
    git config core.hooksPath ./development_utility/git-hooks/
