# Daily Live Report (6 Months)

**Github Workshop Report**

**Date:** 15/01/2025

**Start Time:** 7:00 PM

**End Time:** 9:00 PM

### Learnings from the Workshop:

I have learned the following things from this workshop:

**Version Control System & Git:**

* I learned about version control system

<p style="font-size: 15px;">A version control system is a tool that keeps track of these changes for us, effectively creating different versions of our files. It allows us to decide which changes will be made to the next version (each record of these changes is called a commit), and keeps useful metadata about them. The complete history of commits for a particular project and their metadata make up a repository. Repositories can be kept in sync across different computers, facilitating collaboration among different people. Version control also allows many people to work in parallel.</p>  

### Setting up git:

When we use Git on a new computer for the first time, we need to configure a few things. Below are a few examples of configurations we will set as we get started with Git:

* Our name and email address
* What our preferred text editor is
* That we want to use these settings globally (i.e., for every project)

**Git Help and Manual**

* `$ git config -h`
* `$ git config --help`

### Creating repository

* `$ git init` is used to create and initialize the repository


### Tracking changes

**1. Checking project status:**

```bash
$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)

  lmsquesans.md

nothing added to commit but untracked files present (use "git add" to track)




**Explanation:**

* Explains checking project status with `git status`.
* Includes a code block with the expected output.

**Slide 6**

```markdown
**2. Adding a file to tracking:**

```bash
$ git add lmsquesans.md
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

  new file: lmsquesans.md


**Explanation:**

* Explains adding a file with `git add`.
* Includes a code block with the expected output after adding the file.

**Slide 7**

```markdown
**3. Committing changes:**

```bash
$ git commit -m "Initial commit for lmsquesans.md"
[main (root-commit) f22b25e] Initial commit for lmsquesans.md
 1 file changed, 1 insertion(+)
 create mode 100644 lmsquesans.md


**Explanation:**

* Explains committing changes with `git commit`.
* Includes a code block with the expected output after committing.

**Slide 8** (Optional)

```markdown
### Viewing commit history:

```bash
$ git log

# This will display the commit history


**Explanation:**

* Explains viewing commit history with `git log`.
* Includes a code block with a comment about the output.

**Slide 9** (Optional)

```markdown
### Git Staging Area

<p style="font-size: 15px;">Git works by taking snapshots of changes over the life of project. `git add` specifies what will go in a snapshot (putting things in the staging area), and `git commit` then actually takes the snapshot and makes a permanent record of it (as a commit). 

 
 (![image](/home/abc12/Pictures/Untitled.png)

**Conflicts**
Conflicts occur when two or more people change the same lines of the same file