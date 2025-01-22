
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

```bash
- $ git commit -m "give any message"

[main (root-commit) f22b25e] 
 1 file changed, 1 insertion(+)
 create mode 100644 filename
```
 ```
**Exploring the history**
We use git diff command to know the 
```bash
$ git diff HEAD filename.md
```
Note that **HEAD** is the default option for git diff, so omitting it will not change the command’s output at all (give it a try). However, the real power of git diff lies in its ability to compare with previous commits. For example, by adding ~1 , we can look at the commit before HEAD.

**original file**
```bash

# Guacamole
## Ingredients
* avocado
* lime
* salt
```
- Explanation: This is the original version of the guacamole.md file, which lists the ingredients but does not yet contain any instructions. Instructions

**Change Made to the File**
 ```bash
# Guacamole
## Ingredients
* avocado
* lime
* salt
## Instructions
An ill-considered change

Explanation: In this step, the file is modified by adding the line "An ill-considered change" under the Instructions section.

 Using git **diff** to View the Change
```bash
git diff HEAD guacamole.md

```
**OUTPUT**
``` bash
diff --git a/guacamole.md b/guacamole.md
index b36abfd..0848c8d 100644
--- a/guacamole.md
+++ b/guacamole.md
@@ -4,3 +4,4 @@
 * lime
 * salt
 ## Instructions
+An ill-considered change
```


###Explanation of git diff Output:

  -  diff --git a/guacamole.md b/guacamole.md: This shows the comparison of the file guacamole.md.
  -  index b36abfd..0848c8d: Represents the hashes of the commit before and after the change.
  -  --- a/guacamole.md: The file before the change.
  -  +++ b/guacamole.md: The file after the change.
  -  +An ill-considered change: The + sign indicates that this line was added in the current commit.

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


