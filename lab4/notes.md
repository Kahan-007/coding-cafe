1. --global sets my user name and email across all Git repositories on my computer. If omitted, the setting only applies locally to the current repository.

2. ls -a revealed the hidden .git directory (and .venv) which regular ls hides because it starts with a dot. Inside .git are configuration files and folders (HEAD, config, objects, refs) that store the version history.

3. Git initially offered to track README.md and my lab folders, while .venv/ contains thousands of third-party virtual environment files that I did not write myself.

4. After creating .gitignore, the ignored patterns (.venv/, __pycache__/, *.pyc, .DS_Store) cannot be tracked, and .gitignore itself appears as an untracked file.

5. .gitignore should be committed so that anyone cloning or working on the repository shares the exact same ignore rules and avoids committing unwanted files.

6. README.md moved from "Untracked files" to "Changes to be committed". In the three-places model, it moved from the working directory into the staging area.

7. Git printed the branch name, short commit hash, commit message, and summary showing 2 files changed.

8. The first seven characters are the short commit hash (abbreviated SHA-1 ID). They uniquely identify that specific commit so you can inspect or return to it later.
