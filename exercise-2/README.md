# Exercise-2

In this exercise, you'll practice creating a repository, adding
collaborators, and resolving any conflicts that may arise. You should
work in groups of two or more.

## Set up

To set up the repository, take the following steps:

- **Person 1** should create a new repository on GitHub with a `README.md` file.
- **Person 1** should add **Person 2** as a collaborator to the repository on GitHub
- **Person 1 and Person 2** should _both_ clone the repository to their machine

## Simultaneous Contribution (to create conflict)

Here, we'll see how multiple people contributing to the same project
can create conflicts when integrating changes.

- **Person 1** should edit the `README.md` file by adding a line
  (i.e., `line #2`)that says _My favorite candy is <candy>_
- **Person 1** should then `add` and `commit` those changes, then push
  those changes up to GitHub
- thereafter **Person 2** should then edit the `README.md` file by adding a line
  (i.e., `line #2`)that says _My favorite candy is <candy>_
- **Person 2** should then `add` and `commit` their changes, and
  attempt pushing up to GitHub

At this point, GitHub should prevent **Person 2** from pushing because
they are not working on top of the most recent commit to the project.

## Merging

To allow **Person 2** to replay their changes on top of the most
recent version of the project, they should merge the changes from
the remote:

- **Person 2** should pull and merge changes from GitHub (i.e., `git
  pull --no-edit`). This should **not** work smoothly
  because **Person 1** and **Person 2** edited the **same line of the
  same file**.
- **Person 2** will then have to open the `README.md` file to make
  changes manually and remove conflict markers in the file
- After making the file look **exactly how she wants**, **Person 2**
  should add their changes to the file (with `git add README.md`) and then
  commit the changes (as usual, `git commit -m ...`)
- **Person 2** should now be able to push their (integrated) changes up to GitHub.
