<h1> Git Assignment - Hero Vired <h1>
<h1> Solution for question 1: <h1>
This project demonstrates the process of setting up a Git repository, creating branches, committing changes, and merging branches. The example used is a simple calculator application called CalculatorPlus.

<h1> Table of Contents <h1>
Prerequisites
* Repository Setup
  
* Branch Management

* Feature Implementation

* Merging and Releases

<h1> Prerequisites <h1>
Git installed on your local machine.
  
A GitHub account.

Basic understanding of Git commands and branching.

Repository Setup

<h1> 1. Clone the Repository: <h1>
git clone https://github.com/Ram495-ctrl/git_assignment_HeroVired.git
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
* Add a reviewer and merge post approval.
<h1> 2. Create a New Release: <h1>

Release version 1.0 after merging dev to main.
Create a new branch for additional features.
Implement and test new features.
Merge and release version 2.0.
