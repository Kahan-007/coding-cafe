1. What did `pwd` print?
It printed the absolute path to my current working directory (/home/kahan).

2. What did `ls -al` show that plain `ls` did not?
It displayed hidden files and folders (those starting with a dot, like `.bashrc`) and showed extra details like file permissions, owner, and size.

3. Pick one line from `ls`. What do you think the `Mode` column means?
In Linux, the first column (like `drwxr-xr-x`) shows permissions. It indicates whether the item is a directory ('d') and who has permission to read ('r'), write ('w'), or execute ('x') it.

4. Why does that work from where you are standing? Which kind of path is `coding-cafe/week02`? Absolute or Relative?
It works because the shell looks for the folder starting from my current location (the home directory). It is a Relative path.

5. `mv` did two different jobs above. What were they?
The first `mv` command moved a file into a different directory (`week01/`). The second `mv` command renamed the file while keeping it in the same directory.

6. How many folders are on your `PATH`?
There are 24 folders on my PATH.

7. Write down exactly where your `python` lives:
It lives at `/usr/bin/python3`.

8. Are they the same? If not, why might that be?
They might differ from someone using Windows because Windows installs Python in `AppData`, while Linux (WSL) installs it in standard Unix directories like `/usr/bin/`.

9. What exactly did the shell say? Explain the error in your own words, using the word PATH.
The shell said "pyton: command not found". This means the shell checked all 24 folders listed in my PATH variable top-to-bottom and could not find an executable program named `pyton`.

10. `.venv` did not appear with plain `ls`. Why not?
It did not appear because the folder name starts with a dot (`.`). In Linux, any file or folder starting with a dot is automatically treated as hidden.

11. What changed about your prompt?
My prompt added `(.venv)` to the very beginning, indicating that the virtual environment was active.

12. Is it the same path? If not, what does that tell you about what activation actually did to your PATH?
It is not the same path. Running the activation script temporarily added the `.venv/bin` folder to the very front of my PATH, meaning the shell found the isolated Python before it found the system Python.

13. What is in the second list that was not in the first?
The second list contained `requests` as well as all of its required dependencies (like `urllib3`, `certifi`, `idna`, etc.).

14. Where does `python` point now?
After running `deactivate`, it points back to the global system Python (`/usr/bin/python3`).

15. Find what the recursive flag does. Write it in your own words.
In Linux, the recursive flag (`-R` or `--recursive`) tells the command to list not just the contents of the current folder, but also the contents of every sub-folder inside it, drilling all the way down.

16. What is the difference between what Ctrl + C and Ctrl + Z did?
`Ctrl + C` forcefully interrupted and killed the process. `Ctrl + Z` did not kill the process; it suspended it and paused it in the background, returning control of the terminal to me.
