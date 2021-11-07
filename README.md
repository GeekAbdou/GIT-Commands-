git clone "url.git" (clone repo at local)

git status (get git files status)

git add "dir" / . / * (add file or file) !Note (. or *) for all files

git commit -m "message for commit" (commiting)

git branch 

git push "remoteName" "BranchName" (like master -> origin)

git remote -v (view remote)

git pull "remoteName" "BranchName" (git pull origin master )


git remote add "remoteName" "url.git" 

---

public SSH key 

ssh-keygen -t rsa -b 4096 -c "email@mail.com" 
then add to github account 

ssh -T "email@mail.com"
then authenticate

---

git config --global alias.st status (make st => status "shourtcus")

git config --global alias.cm 'commit -m'

---

git branch "branchName" (create new branch)

git checkout branch "branchName" (to go the new branch)

git branch -b "branchName" (create new branch and go the new branch)

git branch -d "branchName" (delete branch) "Note: "-D" for force delete and "-d" for checking merge before delete"

git branch -m "NewBranchName" (rename current branch)

---

git merge "other branchName" (merge other branchName with current branch)

---

git stash add (add all changes to stash)

git stash add "file name" (saving file at stash)

git stash save "stash name"

git stash pop (pop top element of stash to the working area)

git stash pop "stash@{number}" (pop the spasific stash)

git stash drop (drop / delete top element of stash)

git stash drop "stash@{number}"

git stash apply (apply stash cahanges on the branch and doesn't make anything to the stash)

git stash list   

git stash show "stash@{number}"

git stash clear

---

git restore 

git clean -n 

git clean -f

--- 
git reset head "dir" (remove file or file)

git reset --hard "hash"

git push origin main --force 

---
.gitigone 

to include all files with extension .xxx => *.xxx

to not include exact file and you will ignore all files with same extension => !file.xxx

for whole folder ignoring => file/

for exact file => file.ext

push --force will override 

---

git tag "version x"

git push origin "version x"

git tag -a "version x" -m "anotated tag comment"

git tag -l "version x-search"

git tag -d "version x"

git push origin --delete
