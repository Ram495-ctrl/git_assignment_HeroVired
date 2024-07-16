<h1> Git Assignment - Hero Vired <h1>
  
Collaboration on Github assignment with Kiran
  
<h1> Solution for question 1: <h1>
This project demonstrates the process of setting up a Git repository, creating branches, committing changes, and merging branches. The example used is a simple calculator application called CalculatorPlus.

<h1> Table of Contents <h1>
Prerequisites
  
* Repository Setup
  
* Branch Management

* Feature Implementation

* Merging and Releases

<h1> Prerequisites <h1>
* Git installed on your local machine.
  
* A GitHub account.

* Basic understanding of Git commands and branching.

Repository Setup

<h1> 1. Clone the Repository: <h1>
git clone https://github.com/Ram495-ctrl/git_assignment_HeroVired.git
Cloning into 'git_assignment_HeroVired'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.

<h1> 
2. Navigate to the Project Directory: 
  
cd git_assignment_HeroVired
<h1> Branch Management <h1>
<h1> 1. Create a New Branch: <h1>
    git checkout -b dev
<h1> 2. Create an Application File: <h1>
    nano CalculatorPlus.py
<h1> 3. Track the New File: <h1>
    git add .
<h1> 4. Commit the New File: <h1>
git commit -m "Initial commit of the Calc plus app on Dev"
<h1> 5. Push the Branch to Remote: <h1>
git push origin dev
<h1> 6. Merge dev Branch to main: <h1>
git checkout main
git merge dev
git push origin main
<h1> Feature Implementation <h1>
1. Create a Feature Branch:
 
git checkout -b feature/sqrt

2. Add Square Root Functionality:

nano CalculatorPlus.py

<h1> 3. Commit Changes in Feature Branch: <h1>
git commit -m "Adding sqrt code to the calc plus app in the feature branch"
<h1> 4. Switch to dev Branch and Fix Bugs: <h1>
  
git checkout dev

nano CalculatorPlus.py

git add CalculatorPlus.py

git commit -m "Adding the bug fix for division code in dev branch"

git push origin dev

<h1> Merging and Releases <h1>
<h1> 1.  Merge Feature Branch to dev: <h1>

* Raise a pull request from feature/sqrt to dev.

<img width="1062" alt="image" src="https://github.com/user-attachments/assets/92674683-a71a-4349-beb3-11d2d0b8e039">

* Add a reviewer and merge post approval.

  <img width="1037" alt="image" src="https://github.com/user-attachments/assets/1821df32-1906-4d7f-a16c-b33a67ae4ad3">

<h1> 2. Create a New Release:

Release version 1.0 after merging dev to main.
Create a new branch for additional features.
Implement and test new features.
Merge and release version 2.0.

<img width="801" alt="image" src="https://github.com/user-attachments/assets/f64c968a-83b9-436e-b3ff-b7511156ba1d">


<h1> Solution for question 2: <h1>

<h1> Initialize Git LFS in Your Repository <h1>
git lfs install
  
<h1> Track the Large Files <h1>
  
started track the large file:

git lfs track "*.bin"

![image](https://github.com/user-attachments/assets/0a6283cb-7ead-47b6-bc4c-8f94afd1fe1b)



<h1> Add, Commit, and Push Files <h1>

git add .gitattributes

git add 300MB_Ram.bin

git commit -m "Add large binary file Ram with Git LFS"

git push origin main

![image](https://github.com/user-attachments/assets/fcf22f16-7930-4f63-aaca-a7cc28d41bb4)


Clone the colleague’s repo in lfs folder:

![image](https://github.com/user-attachments/assets/caa51b4e-9c1a-4890-b3c8-24c4a48d77e9)

Pulled contents of his main branch from remote t local cloned repo that also had his binary files:
 
![image](https://github.com/user-attachments/assets/8b0df414-1149-4fa5-afa0-6004c26a4378)

Validated the size and integrity of the friends bin file on my repo and found it to be good:

![image](https://github.com/user-attachments/assets/8b865190-e315-4fc9-a876-5fda8e50d483)



<h1> Solution for question 3: <h1>

<h1> Geometry Calculator <h1>
This repository contains a Geometry Calculator application with features to calculate areas of various shapes. The project follows a branch-based workflow with different features developed in separate branches.

<h1> Branches and Features
1. geometry-calculator Branch

*  Initial Setup: Created the branch geometry-calculator.
*  File Added: calculate_area.py.
*  Initial Commit:

 <h1> Alien@Rahul MINGW64 /e/Devops/Hero vired assignment/Git hub assignment/git_assignment_HeroVired (main)
   
$ git checkout -b geometry-calculator

$ nano calculate_area.py

$ git add calculate_area.py

$ git commit -m "Initial commit of Calculate Area app geometry-calculator branch"

2. feature/circle-area Branch

 * Switch to Branch:

$ git switch feature/circle-area

 * Update Code: Added functionality to calculate the area of a circle.

 * Save Changes:
   
$ git stash

3. feature/rectangle-area Branch

 * Switch to Branch

$ git switch feature/Rectangle-Area

 * Update Code: Added functionality to calculate the area of a rectangle.

 * Save Changes:
   
$ git stash

 <h1> Switched to Feature Circle branch and retrieved the changes, added to tracker and committed:  <h1>

 
<img width="431" alt="image" src="https://github.com/user-attachments/assets/59f49f0b-8cc7-4bad-afed-9a8edec38db6">



<h1> Switched to Feature Reactnagle branch and retrieved the changes, added to tracker and committed <h1> 


<img width="435" alt="image" src="https://github.com/user-attachments/assets/f106be17-ad70-4a7c-9763-6d9ccd9b333e">

<h1> Merge of Feature/Circle code to Dev has been approved by collaborator:


 <img width="1151" alt="image" src="https://github.com/user-attachments/assets/d0599c92-726d-4f7b-ba71-db76aede84e3">

<h1> Merge of Feature/Rectangle code to Dev has been approved by collaborator:

<img width="1117" alt="image" src="https://github.com/user-attachments/assets/6fed24c2-fecd-4c7b-98e4-047229a9fa8e">

<h1> Raised and merged the final merge of Dev branch onto Main branch:

<img width="1025" alt="image" src="https://github.com/user-attachments/assets/b48550ee-69f6-4b40-b853-ecdaafddd580">











