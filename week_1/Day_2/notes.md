# Notes for Day 2

### Table of contents for Today
1. Overview
2. Writing code incrementally
3. Basic git Workflow
4. Problem Solving tips/Debugging

## Overview

* Mon - Thursday: working on core concepts
* Friday is 'Fundamental Friday'
---
* weeks 1-2: Fundamentals
* Weeks 3-5: Web App fundaments
* Weeks 6: Mid-Term
  * simulation of real work dev environment
* Weeks 7-10: Web Frameworks
---
* 4 major solo projects throughout
* 3 Tech Interviews
* Quizzes throughout 
---

## Writing code incrementally

Taking a problem and breaking it down to smaller steps. Then we add all the steps together, to finalize the code.

### Steps to take when starting a new problem:
1) touch to start a new file
2) git init (initialize git)
3) break down your problem into smaller steps. PseudoCoding so that you have  a clear understanding of what the problem calls for. 
4) once you've gotten the different steps browken down, you can then solve each problem independently of one another. 
5) going to be googleing a lot of concepts to figure out how to do something 
6) Best way to debug code, is to console.log everystep to see what's not going through
7) Finally once we have all our independent functions working, we are gong to combine them. This way we know that if something is not working, it's in how it's being implemented.  
---
    Talking About git

    System for tracking changes in source code during software development
    * Remembers the history of our code
      * git hub is different from git. In that GitHub is a service that lets you host repositories on it. 
    * Documents changes with commit messages, listing the author of the changes
    * Chan use a remote git repository to back up out data 
    * We can undo changes we make
    * Makes it easy to collaborate with others on code 

    Git Flow
    
    1) Working directory
        * git add - moves to Staging area
        * adding things to the air lock
    2) Staging area
        * git commit - moves to lovcal repo
          * makes sure to include -m 
        * like an air lock, moviing from inside the ship (working directory) to outside the ship (local repo)
    3) Local Repository (localrepo)
        * git push - moves to remote repo 
    4) Remote Repository 
        * you still need to create a remote repository of the same name on GitHub in order for this to be moved there. 



    git init - initalizes a git repository cretates staginfg area and local repo 

    git status - shows what is in your staging area 

    git log - see previous x num of commits 

    git checkout "String from git log commit" - brings back an older version

    git revert "String from git log commit" - recommits using an older version of the file. 

    git remove - takes things away from staging area. 

  [code . - will open to files that are in a repository in VSCode (outside of Vargant)](https://code.visualstudio.com/docs/editor/command-line)

---


