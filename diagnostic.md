![General Assembly Logo](http://i.imgur.com/ke8USTq.png)

# Unix/CLI Diagnostic

## Challenge

Carry out all of the following tasks using _only the command line_! As is
usually the case, you're welcome to use any resource you can find (except
another student, of course) to reach your answer.

## Navigating the Filesystem

Complete each of following steps, **in order** :

1. Create a new directory called `cli-diagnostic` inside the root directory of
this repository (`unix-cli-diagnostic`).

2. Create a new file inside `cli-diagnostic` called `rhyme.txt`.

3. Open `rhyme.txt` using Atom (via the terminal) and add the following text:

 "The rain in Spain falls mainly in the plain."

 Once you've done this, save the file and quit.

4. Make a directory inside `cli-diagnostic` called `temp`. Inside it, create a new blank file called `temp.md`.

Navigate back up to `unix-cli-diagnostic` directory.
Using Atom, open up `diagnostic.md` and write your answers below (where indicated).

5. Great Work!  Back in the terminal, do  `git status` to view your changes.  What color is the file name?

On branch master
Your branch is up-to-date with 'origin/master'.
Untracked files:
  (use "git add <file>..." to include in what will be committed)

	cli-diagnostic/
	rhyme.txt

nothing added to commit but untracked files present (use "git add" to track)
~/wdi/diagnostics/unix-cli-diagnostic (master)

6. Do `git add <file_name>`  to stage your changes.  Do `git status` again to see the newly staged file.  What color is the file name now?

green
On branch master
Your branch is up-to-date with 'origin/master'.
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

	new file:   cli-diagnostic/rhyme.txt
	new file:   cli-diagnostic/temp/temp.md
	modified:   diagnostic.md

~/wdi/diagnostics/unix-cli-diagnostic (master)

7. Let's commit these changes with `git commit <file_name>` and the commit message of `add temp.md and associated folders`.

8. Navigate back up to `cli-diagnostic`, and delete the `temp` directory (with `temp.md` inside of it). Use `ls` to show the contents of `cli-diagnostic` - was `temp` deleted?

Yes.   Needed the rm -rf command - which is dangerous!

9.  Let's commit our changes, Do  `git status` to view your changes.  Do `git add <file_name>`  to stage your changes.  Commit these changes with `git commit <file_name>` and the commit message of `removegi temp folder`.

## Absolute and Relative Paths

1. Is `/Users/blah_blah/Desktop` a relative path or an absolute path? How do you know?

absolute because it starts with a /

 2. Given:
```sh
~/project
├── css
├── data
├── img
├── js
└── planning
```

If we are in the `project` directory and use `cd planning`, is a relative or absolute path being referenced? How do you know?

relative because planning is relative to where we are at (in project)

3. Now suppose that we have an image file living inside our project. Would we refer to it with an absolute or relative path? Why?

If we are still within project relative
But if we have changed dir to project/planning we would need an absolute to get to /project/planning/*.img

<hr>

You're done! Refer back to README.md.
