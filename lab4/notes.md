1. --global sets my user name and email across all Git repositories on my computer. If omitted, the setting only applies locally to the current repository.

2. ls -a revealed the hidden .git directory (and .venv) which regular ls hides because it starts with a dot. Inside .git are configuration files and folders (HEAD, config, objects, refs) that store the version history.

3. Git initially offered to track README.md and my lab folders, while .venv/ contains thousands of third-party virtual environment files that I did not write myself.

4. After creating .gitignore, the ignored patterns (.venv/, __pycache__/, *.pyc, .DS_Store) cannot be tracked, and .gitignore itself appears as an untracked file.

5. .gitignore should be committed so that anyone cloning or working on the repository shares the exact same ignore rules and avoids committing unwanted files.

6. README.md moved from "Untracked files" to "Changes to be committed". In the three-places model, it moved from the working directory into the staging area.

7. Git printed the branch name, short commit hash, commit message, and summary showing 2 files changed.

8. The first seven characters are the short commit hash (abbreviated SHA-1 ID). They uniquely identify that specific commit so you can inspect or return to it later.

9. The four steps of the Git loop are: edit files in the working directory, check status with git status, stage changes with git add, and commit a snapshot with git commit.

10. README.md gets a special name and root placement because it serves as the front-page overview and guide for the entire repository rather than notes for a single lab.

11. gh auth login generates an authentication token via the browser and stores it in the credential helper so Git authenticates automatically without asking for a password on every push.

12. README.md is shown on the front page because GitHub automatically detects a root README.md file and renders its Markdown into formatted text for visitors.

13. Running git push did not change my local commit history in git log --oneline at all; it simply copied my local commits to the remote repository on GitHub.

14. A repository that does not exist on GitHub lives only on my laptop with no cloud backup or sharing. A private repository on GitHub backs up the history online and lets me grant access only to specific collaborators like my TAs.
