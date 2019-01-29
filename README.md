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
 
