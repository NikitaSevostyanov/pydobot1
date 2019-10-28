I was asked to imagine that I want to implement something cool and I
clearly see the result(The result is the selected repo, only master
branch). I am implementing in part by part. Since I am a good
programmer, each part is implemented in separate branch. And I choose
repository for playing with.

Goals {#goals .unnumbered}
=====

The main goals of the project are:

1.  Repo is suitable for the conditions

2.  Add repo into googlesheet

3.  Repo is unique

4.  The result is the same as choosen repo

5.  Commits directly to master

6.  More than 80% commits containts changes in readme

7.  Commit’s conditions must be maintained

8.  4 branches created

9.  Remove readme

10. Add report

11. Report is useful

12. Remove any folder

Implementation steps {#implementation-steps .unnumbered}
====================

1.  Initializing Git Repo

    -   **“git init”** or ** git clone [repo url]**

    -   If **git init** were used : Connect my repo to remote server
        **"git remote add origin [repo url]**

2.  Add new branch **circleci**

    -   **“git checkout -b circleci”** - add new branch circleci

    -   add file in it **“git add .circleci/config.yml”**

    -   commit changes in the branch **“git commit -m ”remove invalid ci
        setting"**

    -   send this changes to the remote rep **“git push origin
        circleci”**

    -   go to the master branch **“git checkout master”**

    -   edit file **“gedit README.md”**

    -   add new line **“any text”**

    -   add the file **“git add README.md”**

    -   commit changes in the branch **“git commit -m ”update README"**

    -   send this changes to the remote rep **“git push origin master”**

    -   ! But I ,at first, edit README in branch circleci,add it, commit
        and only after that went to master branch and did the actions
        above

3.  Add all needed files, folders in **circleci** or other branch:

    -   **"git checkout circleci**

    -   add folder in it **"git add .circleci/config.yml**( or you can
        add all files at one time : **git add filename filename2
        filename3** or (in folder) **git add folder/filename
        folder/filename2** and etc)

    -   commit changes in the branch **git commit -m “added new
        files-folders”**

    -   send this changes to the remote rep **“git push origin
        circleci”**

    -   change the README.md file. You can see above how to do it.

4.  Do the same actions for examples, other, pydobot branches

5.  If we want to upgrade, modify the existing file we could do it in
    the same way as with README. For example(branch **other**):

    -   Let’s assume, we want to modify file **setup.cfg**

    -   Move to the branch **“git checkout other”**

    -   Change the file **“gedit setup.cfg”** ( or if you change the
        file before, just copy it in Local Rep)

    -   add the file **“git add setup.cfg”**

    -   commit changes in the branch **git commit -m “prepare for pyPip
        package”**

    -   send this changes to current rep **“git push origin **other**”**

    -   send this changes to the remote rep **“git push origin master”**

6.  You can use command **“git config -global credential.helper store”**
    in order not to type password and login every time you push or pull

7.  To copy files from your project to your local repository in order to
    work with it further, you should type command like this: **cp
    /home/Desktop/pydobot1/pydobot/dobot.py**

8.  If you want to delete branch both in Local or in Remote Rep, type
    this 2 commands: **“git push -d remotename branchname”** and **“git
    branch -d branchname”**

9.  If you want to delete some file either in Local and in Remote Rep,
    type this 3 commands: **“git rm filename”** , **“git commit -m ?”**
    , **“git push origin branch”**

10. if you want to move some file or folder in other directory in your
    rep then use this: **“git mv FileDirName FileDirNameDestination”** ,
    **“git commit -m smth” ** and **"git push origin branch** ,
    /home/Desktop/hw\_git/Report.tex

11. To merge all branches to the master: **“git checkout master” ** and
    then **“git merge NranchName”** . If there are conflicts, you should
    resolve them manually.


