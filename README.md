📝 Daily Live Report (6 Months)
📊 GitHub Workshop Report

📅 Date: 15/01/2025

⏰ Start Time: 7:00 PM

⏳ End Time: 9:00 PM

---

🔍 Learnings from the Workshop:

🌐 Version Control System & Git:

A version control system is a tool that tracks changes made to files, effectively creating different versions of the files over time. It allows us to:
- Decide which changes will be included in the next version (each record of these changes is called a commit).
- Store useful metadata for each commit.
- Maintain a complete history of commits and their metadata, forming a repository.
- Synchronize repositories across different computers, enabling collaboration among multiple people.

⚙️ Setting Up Git:

When using Git for the first time on a new computer, some configurations are necessary:

```bash
$ git config --global user.name "Your Name"
$ git config --global user.email "your.email@example.com"
```

Git Help and Manual:

```bash
$ git config -h
$ git config --help
```

📂 Creating a Repository:

```bash
$ git init
```

📜 Tracking Changes:

1. If we check the status of our project, Git tells us that it's noticed the new file:

```bash
$ git status

On branch main
No commits yet
Untracked files:
   (use "git add ..." to include in what will be committed)

    file

nothing added to commit but untracked files present (use "git add" to track)
```

Git Add Command:

```bash
$ git add file-name

On branch main
No commits yet
Changes to be committed:
  (use "git rm --cached ..." to unstage)

    new file:   filename
```

Git Commit Command:

```bash
$ git commit -m "give any message"

[main (root-commit) f22b25e] 
  1 file changed, 1 insertion(+)
  create mode 100644 filename
```

Exploring the History:

```bash
$ git diff HEAD filename.md
```

Original File Example:

```
# Guacamole
## Ingredients
* avocado
* lime
* salt
```

Change Made to the File:

```
# Guacamole
## Ingredients
* avocado
* lime
* salt
## Instructions
An ill-considered change
```

Git Diff Output:

```
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

Explanation of git diff Output:

- `diff --git a/guacamole.md b/guacamole.md`: This shows the comparison of the file guacamole.md.
- `index b36abfd..0848c8d`: Represents the hashes of the commit before and after the change.
- `--- a/guacamole.md`: The file before the change.
- `+++ b/guacamole.md`: The file after the change.
- `+An ill-considered change`: The `+` sign indicates that this line was added in the current commit.

Push the File into Repo:

```bash
$ git push origin main
```

Git Log:

```bash
$ git log
```

Staging Area:

Git takes snapshots of changes over the life of a project. The `git add` command specifies what will go into a snapshot (putting things in the staging area), and `git commit` actually takes the snapshot and makes a permanent record of it (as a commit). If you don't have anything staged when you type `git commit`, Git will prompt you to use `git commit -a` or `git commit --all`. However, it's almost always better to explicitly add things to the staging area, because you might commit changes you forgot you made.

📌 Illustrative Diagram:

![Diagram](https://github.com/user-attachments/assets/639861d6-1306-49ab-aaf7-1a2f81d5fa62)

Conflicts:

Conflicts occur when two or more people change the same lines of the same file.
