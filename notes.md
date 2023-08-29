git commit -m "message" --> commits current staged files to current branch. 
git log --> shows operations performed with time, date and user details. (with new hash every commit) 

git init - initializes current repository as working environment
Initialized empty Git repository in C:/Mydocs/Learning/learning-git-github-2421501-01_02b/.git/


staging  - add command
git add . / git add Filename / git add -A  - adds to proceed the changes for committing, -A & . means all the files in directory.  


git status --> shows information of current branch 

git restore filename 
git restore .    --> reverts back the changes 

git restore -S .\README.md     

git restore <filename>   -> contents are reverted back 

Sensitive info, system files are not required to be uploaded. 
ignore files -  arent uploaded to github 


adding a .gitignore files with names of restricting files and commiting the gitignore file.
Next time we add that sensitive info file it will not be in staging area. 


git rm -r --cached .
--> deletes all the cached files over course of multiple commits 

Removing
git rm filename --> deletes and stages
for Undo op: git restore -S . >> git restore .

git mv index.html home.html
--> renames and stages
Undo: by renaming again or unstage and restore 

git diff - to know the differences. 

git log --oneline --> shorter messages 

ammend -- ammend the hitsory and edit the file
-ammend option 
--no-edit : no updation in commit msg 

git commit -amend -m " msg" to update with previous commit and avoid multiple instances of commits unnecessarily 

git reset "hash value" - rewinds the commit/ doesnt change the updated content , only reverts back particular changelist. 
git config --global core.editor "'C:\Program Files\Notepad++\notepad++.exe' -nosession -notabbar"  - setting the notepad as default editor 


git rebase: take commits from one branch to apply to another. or change history to much earlier commits without affecting the files./reorganise the order in which commits are made.
git rebase -i HEAD~3 - goes back in the same branch to last 3 commits position.
git rebase -i --root - shows all commits. 

git checkout -b "new name"     

Merging: 
git merge branch-bhc (from branch_bhc to master it will get merged 

git branch -delete "NAME"      

git flow:
Feature/fix branch
make changes
merge to master
delete old branch 

git checkout master - to switch branches

git stash :
stores current change for later use and reverts back to original 

git stash
git stash list
git stash apply (restore/add-commit)
git stash pop (applies the changes from stash) - last item on stash - 

git clean - removes all untracked files from directories 

github: storage service in cloud.  compared to git, it provides a collaborative platform
project management tools, creating and assign issues 

adding local changes to github by remote command:

git remote add 

git remove add NAME URL
git push -all
git push -u origin name of branch 