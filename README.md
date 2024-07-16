<h1> Introduction:
  
  Collaboration on Github assignment with Kiran
  
  Create a git_assignment_HeroVired repository 
cloned the new repo to local:
Alien@Rahul MINGW64 /e/Devops/Hero vired assignment/Git hub assignment/git_assig
$ git clone https://github.com/kiran-umesh/git_assignment_HeroVired.git
Cloning into 'git_assignment_HeroVired'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.
Created new branch "dev":
Alien@Rahul MINGW64 /e/Devops/Hero vired assignment/Git hub assignment/git_assignment_HeroVired (main)
$ git checkout -b dev
Switched to a new branch 'dev'
Created the app file:
Alien@Rahul MINGW64 /e/Devops/Hero vired assignment/Git hub assignment/git_assignment_HeroVired (dev)
$ nano CalculatorPlus.py
Added it for tracking
Alien@Rahul MINGW64 /e/Devops/Hero vired assignment/Git hub assignment/git_assignment_HeroVired (dev)
$ git add .
warning: in the working copy of 'CalculatorPlus.py', LF will be replaced by CRLF the next time Git touches it
Committed the file for the first time
Alien@Rahul MINGW64 /e/Devops/Hero vired assignment/Git hub assignment/git_assignment_HeroVired (dev)
$ git commit -m "Initial commit of the Calc plus app on Dev"
[dev 557cee2] Initial commit of the Calc plus app on Dev
 1 file changed, 47 insertions(+)
 create mode 100644 CalculatorPlus.py

Pushed it to remote repo:
Alien@Rahul MINGW64 /e/Devops/Hero vired assignment/Git hub assignment/git_assignment_HeroVired (dev)
$ git push origin dev
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 24 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 685 bytes | 685.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/Ram495-ctrl/git_assignment_HeroVired/pull/new/dev
remote:
To https://github.com/Ram495-ctrl/git_assignment_HeroVired.git
 * [new branch]      dev -> dev
Switched to Main and merged the Dev branch to main:
Alien@Rahul MINGW64 /e/Devops/Hero vired assignment/Git hub assignment/git_assignment_HeroVired (dev)
$ git switch main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
Alien@Rahul MINGW64 /e/Devops/Hero vired assignment/Git hub assignment/git_assignment_HeroVired (main)
$ git merge dev
Updating 0e495e6..5d06b69
Fast-forward
 CalculatorPlus.py | 47 +++++++++++++++++++++++++++++++++++++++++++++++
 1 file changed, 47 insertions(+)
 create mode 100644 CalculatorPlus.py

Pushed main to remote repo:
Alien@Rahul MINGW64 /e/Devops/Hero vired assignment/Git hub assignment/git_assignment_HeroVired (main)
$ git push origin main
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Ram495-ctrl/git_assignment_HeroVired.git
   0e495e6..5d06b69  main -> main
created release version 1.0

create new branch feature/sqrt
Alien@Rahul MINGW64 /e/Devops/Hero vired assignment/Git hub assignment/git_assignment_HeroVired (main)
$ git checkout -b feature/sqrt
Switched to a new branch 'feature/sqrt'
Updated code to add sqrt functionality:
Alien@Rahul MINGW64 /e/Devops/Hero vired assignment/Git hub assignment/git_assignment_HeroVired (feature/sqrt)
$ nano CalculatorPlus.py

Committed changes in Feature branch before moving to Dev branch for working bug fix, to keep the branch clean and up-to-date:
Alien@Rahul MINGW64 /e/Devops/Hero vired assignment/Git hub assignment/git_assignment_HeroVired (feature/sqrt)
$ git commit -m "Adding sqrt code to the calc plus app in the feature branch"
[feature/sqrt c6e99f7] Adding sqrt code to the calc plus app in the feature branch
 1 file changed, 4 insertions(+), 4 deletions(-)
Updated file on Dev branch to add bug fix for division code:
Alien@Rahul MINGW64 /e/Devops/Hero vired assignment/Git hub assignment/git_assignment_HeroVired (feature/sqrt)
$ git switch dev
Switched to branch 'dev' 
Alien@Rahul MINGW64 /e/Devops/Hero vired assignment/Git hub assignment/git_assignment_HeroVired (dev)
$ nano CalculatorPlus.py
Alien@Rahul MINGW64 /e/Devops/Hero vired assignment/Git hub assignment/git_assignment_HeroVired (dev)
$ git add CalculatorPlus.py
Alien@Rahul MINGW64 /e/Devops/Hero vired assignment/Git hub assignment/git_assignment_HeroVired (dev)
$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   CalculatorPlus.py
Alien@Rahul MINGW64 /e/Devops/Hero vired assignment/Git hub assignment/git_assignment_HeroVired (dev)
$ git commit -m "Adding the bug fix for divison code in dev branch"
[dev 415cece] Adding the bug fix for divison code in dev branch
 1 file changed, 4 insertions(+)
Merged the feature code for sqrt onto Main branch by raising pull request and was approved by kiran-umesh.
Committed the code for testing and pushed to remote:
Alien@Rahul MINGW64 /e/Devops/Hero vired assignment/Git hub assignment/git_assignment_HeroVired (dev)
$ git push origin dev
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 24 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 403 bytes | 403.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Ram495-ctrl/git_assignment_HeroVired.git
   5d06b69..415cece  dev -> dev
Raised pull request to merge Feature code to Dev adding a reviewer
Merged the code post approval
Created a new release with V2.0



