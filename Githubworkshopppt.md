<!-- Slide 1 -->
# Introduction to Git
**Software Carpentry - Git Novice**

Learn the basics of version control and how to use Git for tracking changes in your projects.

---

<!-- Slide 2 -->
# What is Version Control?
- **Version Control**: A system that records changes to files over time.
- It allows you to **track changes** to files, collaborate with others, and undo mistakes.

---

<!-- Slide 3 -->
# What is Git?
- **Git**: A distributed version control system.
- Git tracks changes to your files and stores them in a repository.
- It allows you to **collaborate** with others and work on multiple versions of your project simultaneously.

---

<!-- Slide 4 -->
# Benefits of Using Git
- Track changes over time.
- Collaborate with others without worrying about overwriting work.
- Undo mistakes and restore previous versions of files.
- Work on multiple features or bug fixes in parallel using branches.

---

<!-- Slide 5 -->
# Setting Up Git
To get started with Git, you need to **install** it and set up your username and email.

```bash
git config --global user.name "Your Name"
git config --global user.email "youremail@example.com"

```

<!-- Slide 6 -->

  # Creating a Repository

To create a new Git repository, use:
```bash
git init
```
This initializes a new Git repository in the current directory

<!-- Slide 7 -->

# Staging Files

Staging: Adding files to Git's "staging area" before committing.
To add files to the staging area:
```bash
git add <file-name>
```


<!-- Slide 8 -->
Committing Changes

    Commit: Save changes to your repository.
    Each commit requires a commit message.
```bash
git commit -m "Message describing the changes"
```
<!-- Slide 9 -->
Viewing History

    To see the history of commits:
``` bash
git log
```
    This shows a list of all previous commits.

<!-- Slide 10 -->
Branching in Git

    Branching allows you to work on different tasks in parallel.
    To create a new branch:
``` bash
git branch <branch-name>
```
<!-- Slide 11 -->
Switching Branches

    To switch between branches:
``` bash
git checkout <branch-name>
```
<!-- Slide 12 -->
Merging Branches

    Merging: Combine changes from one branch into another.
``` bash
git merge <branch-name>
```
<!-- Slide 13 -->
Cloning a Repository

    To copy an existing Git repository to your local machine:
``` bash
git clone <repository-url>
```
<!-- Slide 14 -->
Pushing Changes to a Remote Repository

    To upload your local changes to a remote Git repository (e.g., GitHub):
``` bash
git push origin <branch-name>
```
<!-- Slide 15 -->
Pulling Changes from a Remote Repository

    To fetch and integrate changes from a remote repository:
```bash
git pull origin <branch-name>
```
<!-- Slide 16 -->
Resolving Conflicts

    Merge Conflicts occur when changes in two branches conflict.
    To resolve a conflict:
        Git marks the conflicting sections in the file.
        Edit the file to resolve the conflict.
        Then, commit the changes.



<!-- Slide 17-->
Conclusion

    Git helps you track, manage, and collaborate on projects.
    Using commands like git add, git commit, and git push, you can manage your project history and collaborate with others efficiently.
    Branching and merging allow for effective parallel development.

<!-- Slide 18-->


### **Explanation of the Slides**:
1. **Slide 1 (Introduction)**: Introduces the topic of version control and Git.
2. **Slides 2–4**: Explains what version control and Git are, and why they are useful.
3. **Slides 5–7**: Covers the basic Git setup process, staging files, and committing changes.
4. **Slides 8–10**: Introduces the concepts of viewing commit history, branching, and switching branches.
5. **Slides 11–13**: Discusses merging branches, cloning repositories, and pushing changes to remote repositories.
6. **Slides 14–16**: Explains how to pull changes, handle conflicts, and use the `.gitignore` file.
7. **Slide 17(Conclusion)**: Summarizes the key points.
8. **Slide 18(Next Steps)**: Encourages further practice and learning.

---


