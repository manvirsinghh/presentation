# 📝 Daily Live Report (6 Months)

## **📊 GitHub Workshop Report**
**📅 Date:** 15/01/2025  
**⏰ Start Time:** 7:00 PM  
**⏳ End Time:** 9:00 PM

---

### **🔍 Learnings from the Workshop:**

I have learned the following concepts during this workshop:

#### **🌐 Version Control System & Git:**
- A **version control system** is a tool that tracks changes made to files, effectively creating different versions of the files over time. It allows us to:
  - Decide which changes will be included in the next version (each record of these changes is called a **commit**).
  - Store useful metadata for each commit.
  - Maintain a complete history of commits and their metadata, forming a **repository**.
  - Synchronize repositories across different computers, enabling collaboration among multiple people.
  - Allow parallel work among team members.

> **💡 Note:** Version control systems facilitate structured and efficient team collaboration.

---

#### **⚙️ Setting Up Git:**
When using Git for the first time on a new computer, some configurations are necessary:
- **Configuring user details** (name and email address):
  ```bash
  $ git config --global user.name "Your Name"
  $ git config --global user.email "your.email@example.com"



**Git Help and Manual**
- $ git config -h
- $ git config --help
 
📂 **Creating a Repository:**
- $ git init is used to create and initialize the repository

 📜 **Tracking Changes:**
  1. If we check the status of our project a Git tells us that it’s noticed the new file:
    
  - $ git status
``` bash
On branch main

No commits yet

Untracked files:
   (use "git add <file>..." to include in what will be committed)

	file

nothing added to commit but untracked files present (use "git add" to track)
```

The “untracked files” message means that there’s a file in the directory that Git isn’t keeping track of. We can tell Git to track a file using git add:
- $ git add file-name
``` bash
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   filename
```

Git now knows that it’s supposed to keep track of filename.md, but it hasn’t recorded these changes as a commit yet. To get it to do that, we need to run one more command:
BASH

- $ git commit -m "give any message"
 ```bash
[main (root-commit) f22b25e] 
 1 file changed, 1 insertion(+)
 create mode 100644 filename

 ```
 Push the file into repo
- $ git origin  main
   
If we want to know what we’ve done recently, we can ask Git to show us the project’s history using git log:


- $ git log

  **Staging area**
  Git as taking snapshots of changes over the life of a project, git add specifies what will go in a snapshot (putting things in the staging area), and git commit then actually takes the snapshot, and makes a permanent record of it (as a commit). If you don’t have anything staged when you type git commit, Git will prompt you to use git commit -a or git commit --all, which is kind of like gathering everyone to take a group photo! However, it’s almost always better to explicitly add things to the staging area, because you might commit changes you forgot you made.

📌 **Illustrative Diagram:**
  
 (![image](https://github.com/user-attachments/assets/639861d6-1306-49ab-aaf7-1a2f81d5fa62)


**Conflicts**
Conflicts occur when two or more people change the same lines of the same file.
