                                             Git Cheatsheet

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

71ab1ffdde2b5c87dd42ffbc0dd0dcfe4a20675f

All About remote Pushing and Remote command Lines

13. 'git diff commit1 commit2 → gives the difference of all file changes between two commits
14 git commit -n *<your commit message>→ If we want to avoid opening a text editor like vim/nano to
add commit message we can use this following command
15. "'git remote → list down all the remote connection names
16. Remote connection → It helps you to link two git repositories for uploading and downloading changes
from each otherwise
17. 'git remote add <name of remote> <link of the remote>`: this command helps us to add a new link to the
remote repo and give a name to it
18. 'git remote rm <name of remote>`: this command deletes a remote connection
19. 'git remote rename <olanme> <newname>`: this command remanes the remote connection
Note: The name of the remote connection is always used to establish communication between the repos.





My Working and Staging Area Should be clean in order to pull the origin


### Recommended practice to do
- make changes
-git add <file>
-git commit
-git pull
-git push
So here we will try to push our code in case of merge conflict






<!-- BRANCHES -->

git checkout -b <Branch Name>

git will  Never Know how Many Branches are there until unless a commit from that branches will be committed


Complete Wrong Way Of Pushing The code

Suppose You have changes in the remote repository which is not Included in my Local repo and Suppose we Have Created A new Feature Branch and Added an feature in the feature Branch so we will Not do Like Merge Feature Branch to the master branch and then pull the changes from the remote repo and then push it to the remote repo



SO Best Way of Merging New Feature is:


First Pull all the code into the local master Branch 
and then push the feature branch direclty into the its remote and in the remote we will se the pull request 

{Pull request:- It is a way of requesting a branch i.e most of the time master to review the feature or the code i want to add to your main master code} and then merge it 


It is Loc=gical that why Merging your Feature Branch to the Master is Bad Because No One will have see the changes so it Is bad Conventional to the Push the whole master and the mainter will never get to know about the changes and it is a Bad Practice



Now WE ARE GOING TO DICUSS HOW WE ARE GOING TO CONTRIBUTE TO OPEN SOURCE PROJECTS AS WE ARE NOT THEIR COLLABORATORS SO THEY DON'T TRUST US WHICH IS VALID ALSO BECAUSE THEIR CODE IS VALUABLE TO THEM 

SO OUR AIM IS HOW CAN WE BECOME ||CONTRIBUTOR || 

1.Fork the repo which you want to contribute to

2.Clone that repo or bring it to the local repo and as it is a repo means it is already .git folder in it or initialized

3.Make the changes or add the feature and stage it commit it and push it to your Remote forked Master or to the branch in which you want to push in remote repo


4.Create A Pull request to the orignal owner of the repository

5.You can search Your Pr by going into pull request and is:pr is:oopen/closed author:authorName