# Git Assignment — Answers


## Q1:
1. A terminal is a space where you type commands to perform any operation, not by clicking everything. This is the difference between terminal and clicking through folders.
2. To list all the files including hidden use : ls -a
   To create a folder use : mkdir
   To move to that folder use : cd "path"
3. cd . . takes you back to the previous directory and cd ~ takes you to very base directory

## Q2:
4. Version Control is a method that tracks your code, files over the period of time and maintain a history. In a company where a team is working on same project and sharing code files, in that scenario we use version control so that it maintain a histoy and help to compare or restore any previous changes.
5. Git is a tool, you download and use it to write git commands totrack your folder/code files whereas Github is a platform that provides you an interface for doing things.
6. Github provides option like "Create pull Requests" , "Create Merge Requests" , "Report Issues and Assign tasks"
7. Local repository can only be accessed by you and stored locally whereas remote repo can be accessed from anywhere as it is stored on cloud.

## Q3:
8. Head is a pointer that looks for the recent commit and it move the pointer to next when you switch to next branch.
9. .gitignore file tells what files not to track when you push code to github

## Exercise 2.2.6
We commited A+B together and C seperate and we normally do this to keep similar modules/code or feature together and commit different module separatly to avoid conflicts or for better undersatnding.


## Exercise 2.3.6
If we made local commit first without pulling, then we will remain 1 step backward from the that branch, and that branch will be 1 step forward from us.


## Exercise 3.1.9
We can see in the terminal that it was Fast Forward, it means that it has just moved the head pointer from one branch to another.


## Exercise 3.2.15
1. The conflict heppened because we made changes to same file and in same line from 2 different branches and when we merged them it shows conflict and asked which version to keep or discard.
2. No there would be no conflict if the two branches edited different lines of team.txt 
3. Similarly there would be no conflict if one branch edited team.txt and the other edited about.md because both are different files.


## 4.1.13
1. we made a pull request so that others or team lead can review the code, chnages we made and test the code before merging into main, instaed of directly merging to main branch.
2. 
   . Reviewer should check that whether the code is working as expected or is there any bug.
   . Reviewer should also check conflicts and resolve them
3.  
   . Fast-forward merge moves the branch head pointer forward to oanother branch without creating a new merge commit.
   . Merge commit creates a new commit to combine the histories of both branches.



## Scenario A: 
There will no conflict because both Ahmed and Sara worked on different lines in same file, git will merge them without a conflict

## Scenario B: 
There will no conflict because both Ali and Fatima worked on different files, so git will merge them without a conflict

## Scenario C:
There will be a conflict in this scenario becasue Dec A and Dev B both chnaged the same line of code, so git will show a conflict which version to keep or which to delete. The conflict will look like:

```<<<<<<<< HEAD
DEBUG = True
=======
DEBUG = False
>>>>>>> feature-branch
```

## Scenario D:
1. First i will open the index.html file and look for conflicts
2. Resolve the conflict by keeping one version or by combining both 
3. Commit Merge 
4. Verify after merge 

## Scenario E:
This is a good practice to take pull everytime you start working so your code will keep up to date and to avoid conflicts. 
if he avoids git pull and start working so after completing his side of work when he push the code and his team member has already made chnages on same files then git will raise many conflicts between both versions.