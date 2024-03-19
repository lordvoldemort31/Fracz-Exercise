# Fracz git exercises

## Master

Used git master to start the master exercise

    git start master
    git verify

## Commit-one-file

add any of the file in staging 
Once the file is staged, we can commit it using the git commit command.

    git add A.txt
    git commit -m "for A"
    git verify

## commit-only file-staged
start this exercise by using " git start commit-only file-staged " command then check which files are currently staged for commit. we can use the git status command to see the status 
since we have two files staged for commit and we only need to commit one ,i want to commit B.txt. You can unstage A.txt using the git reset A.txt commend then commit it then verif


    git start next
    git status
    git reset A.txt
    git commit -m "message"

## ignore them

touch .gitignore will create a .gitignore file then add patterns to it to ignore files then add your file to stage and then commit

    git start next
    touch .gitignore
    cat > .gitignore
    _.exe
    _.o
    \*.jar
    libraries/
    git add .
    git commit -m "ignore"
    git verify

## chase branch

 First, check which branch we are currently on by running "git branch"
"git merge escaped" command merges the changes from the "escaped" branch into the current branch

 
    git start next
    git branch
    git merge escaped
    git verify

## merge-conflict

there was a conflict in equation.txt , edit 2+3=5 in this file then commite and then merge branches

    git start next
    git merge
    cat equation.txt
    git add .
    git commit -m "msg"
    git verify

## save your work

using git stash commit without save work then remove bugs then commit the changes.

    git start next
    git stash
    cat bug.txt
now edit bug file

    git add . 
    git commit -m "msg"
    git stash pop

now add finally , finished it! in bug file

    git add .
    git commit -m "msg"
    git verify

## change-bransh-history
exercise can be completed easily by using "git rebase hot-bugfix" command only

    git start next
    git rebase hot-bugfix
    git verify

## Remove-ignored

"git rm ignored.txt " this command removes the file "ignored.txt"

    git start next
    git rm ignored.txt
    git add .
    git commit -m "msg"
    git verify

## Case-sensitive-filename

"git mv FILE.txt file.txt" command renames the file from "FILE.txt" to "file.txt"

    git start next
    git mv FILE.txt file.txt
    git add . 
    git commit -m "lowercase-done"
    git verify

## fix typo

    git start next
    cat file.txt

go to file and correctspelling mistake of world

    git add . 
    git commit --ammend -m "Add Hello world"
    git verify

"git commit --ammend -m "Add Hello world"" command amends the previous commit by replacing its commit message with "Add Hello world". It includes the changes that were staged with the previous commit, effectively fixing the typo

## forge-date

can be easily solved by using single command " git commit --amend --date="1987" -m "date" "

    git start next
    git commit --amend --date="1987" -m "date"
    git verify

## fix-typo-old

    git rebase -i HEAD^^
    git commit --amend
    git rebase --continue
edit in file

    git add .
    git verify
