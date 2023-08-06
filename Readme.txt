1. `git init → Powers your folder to be managed by git, and initialises a new empty
repository. It also creates a .git folder that has all the relevant logic to manage
versions of your project.

2. Working Area → There can be a bunch of files that are not currently handled by git.
It means that changes done or to be done in those files are not managed by git yet. A file
which is in working area is considered to be not in the staging area. When we do 'git status"
and we see abunch if untracked files then these are actually called to be in the working area.

3. `Staging area → What all files are going to be part of the next version that we will create.
This staging area is the place where git knows what changes will be done from the last version to
the next version.

4. "Repository Area → This area actually contains the details of all you previous registered version.
And the files in this area, git already manages them and knows their version history.


5. "git add <file> → moves file from working area to staging area

6. `git rm --cached <file> → moves file back from staging area to working area

7. 'connit → Commit is a particular version of the project. It captures a snapshot of the project's staged
changes and creates a version out of it.


8. 'git commit → registers staging changes to a commit







9. 'git log → list downs all the commits of the repository

12. Diff between git rm and git restore
ans: if you want to move the whole file back to the untracked state, then we do git rm, otherwise if we
just want the changes to be moved in working area or staging area then we git restore. 
