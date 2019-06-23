# GitPractice

Commands for Git upload

git remote set-url origin new_url      // for changing Repositry

git remote --verbose | grep origin       //to check current repositry

=> create new repositry
git init
git remote add origin <URL>
git add .                                // to add all projects
git add nameOfProject                    // to add specific project
git commit -m "put your commit message here"
git push -u origin master                 // to push your code on repositry



git add .          // to add all the file in staging area
git commit -m "MESSAGE"

git log // For look at commit log

git log --author="NameOfDeveloperOrProgrammer"

git status // Show status of working directory

git diff   // it shows difference between Working Directory File and Repositry Directory File

git diff --staged // it shows difference between Staging Directory File and Repositry Directory File

git rm third.txt // remove file from folder [ after Removing the file please commit the file to take a snapshot]

============ MOVE AND RENAME FILE =================

First Rename The File Mannulally Using F2

Then Use Two Command [ First git add home.txt { then } git rm First.txt ]   // it means you rename the First.txt into Home.txt Now Commit With A Message

                                     OR
[ git mv First.txt Home.txt ]   // Command To Rename Directly

git mv second.txt FOLDERNAME/REname The Second.txt file    // For Move To Another Folder And Rename
eg => git mv second.txt MyFolder/RenameSecondFile.txt

git commit -am "MESSAGE"  // Directly Commit to Repositry Escape the { git add } line [ Works Only On Edit Not Delete ]

================Checkout [ Means From Reposity to Working Directory ] =========
git checkout -- index.html  [ move old index.html file to currrupted index.html file in working directory ]

 =========== UNSATGE FILE ==========
 
 git reset HEAD index.html  [ move back from staging area to Working Directory ]
 
 ===== GETTING OLD VERSION FROM THE REPOSITRY ====
 
 git checkout --{commit number First Few Digits } FileName
 
 
 ################  CREATE Branches #################
 By default branch is master branch
 
 1- for create branch use command
     git branch vasu-branch-name
   
Note:  After creating branch with above command you have to use "checkout" command to work on this if you don't want to checkout and work on the new branch then use command
     git checkout -b vasu-branch-name
     
 2-  To see all branches
      git branch -a
      
 3- to switch to diff branch
       git checkout vasu-branch-name
       
 4- for deleting branch
          Just go to master branch first using command "git checkout master" then use command
          git branch -D vasu-branch-name
          
 ###############  MERGING Branches #################
 
 Go to your master branch and use below command
     git merge vasu_branch1
     
 
 
