# Fracz git exercises

## Master

Used git master to start the master exercise

    git start master
    git verify

## Commit-one-file

add any of the file in ataging area

    git add A.txt
    git commit -m "for A"
    git verify

## commit-only file-staged

    git start next
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

    git start next
    git branch
    git merge escaped
    git verify

## merge-conflict

there was a conflict in equation.txt , edit 2+3=5 in this file then commite and then merge branches

    git start next
    git merge
    cat equation.txt
    2+3=5
    git add .
    git commit -m "merge"
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

    git start next
    git rebase hot-bugfix
    git verify

## Remove-ignored

 can remove the file from working directory as well as the staging area by the command below.

    git start next
    git rm ignored.txt
    git commit -m "msg"
    git verify

## Case-sensitive-filename

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

## forge-date

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
