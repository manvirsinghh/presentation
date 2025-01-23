📝 Daily Live Report (6 Months)
📊 GitHub Workshop Report

📅 Date: 15/01/2025

⏰ Start Time: 7:00 PM

⏳ End Time: 9:00 PM

---

🔍 Learnings from the Workshop:

 # **Summary and setup**

# Example Scenario: Group Project for University

 ## Imagine a team of students working on a group project report:

  ###  Without Version Control:
        Alice writes the introduction in report.docx and emails it to Bob.
        Bob adds the body section and sends the file back to Alice.
        Meanwhile, Charlie edits the same original report.docx to add the conclusion.
        Problem: When all three versions are combined, some sections may be overwritten, duplicated, or lost entirely. It’s also unclear who made which changes and when.

   ###   With Git:
        Alice, Bob, and Charlie each clone the same repository of the report.docx file.
        Alice works on the introduction, Bob on the body, and Charlie on the conclusion simultaneously.
        They commit and push their changes to the repository. If there’s a conflict (e.g., two people editing the same part), Git flags it for resolution.
        Solution: Everyone’s contributions are seamlessly merged, and the entire team can see a clear history of edits.

  ## **Prerequisites**

 # - Text Editor

When you're writing code, it's nice to have a text editor that is optimized for writing code, with features like automatic color-coding of key words. 
Nano is one of  the editor .it should be pre installed .In case if it is not pre installed then use these set of commands to install it 

### Install Nano on Debian/Ubuntu-Based Systems

Run the following commands  in terminal(Ctrl+Alt+T)to install Nano:

```bash
sudo apt update         # Update your package list
sudo apt install nano   # Install Nano
nano --version          # Verify the installation

```
 Here I have shown demonstration of installation process:-

![nano](https://github.com/user-attachments/assets/84bcf759-63ad-442a-b890-d6b3c6d2fbeb)


  # - Installing git

  

Git is a version control system that lets you track who made changes to what when and has options for easily updating a shared or public version of your code on github.com. You will need a supported web browser.

You will need an account at github.com for parts of the Git lesson. Basic GitHub accounts are free. We encourage you to create a GitHub account if you don't have one already. 


For Debian/Ubuntu run 
``` bash
sudo apt-get install git
```

Demonstration of git installation
![git](https://github.com/user-attachments/assets/1bd49cf9-dbce-45f3-a625-5b1509b9c0dd)


**Creating a GitHub Account**

    1 Go to https://github.com and follow the “Sign up” link at the top-right of the window.
    2. Follow the instructions to create an account.
    3. Verify your email address with GitHub.
    4.Configure multifactor authentication (see below).

   # Multi-Factor Authentication (MFA) on GitHub

## **Why is MFA Important?**
- Passwords alone are not enough because they can be:
  - **Guessed**, **stolen**, or **reused** from other breaches.
- If someone gets your GitHub password, they could:
  - Access your code, projects, or even harm open-source communities.
- **Solution**: Multi-Factor Authentication (MFA) adds a second layer of security.

---

## **What is MFA?**
MFA ensures that even if someone has your password, they need a second form of verification, such as:
1. A **code** from your phone.
2. A **hardware security key**.

---

## **How to Set Up MFA on GitHub?**
You have several options based on your convenience:

### **1. Use an Authenticator App**
- If you already use apps like **Google Authenticator** or **Duo Mobile**, just add GitHub to the app.
- The app generates one-time codes for secure login.

### **2. Don’t Have an Authenticator App?**
No problem! You can:
- **Receive login codes via SMS** (check if your country supports this).
- **Use a hardware security key** like **YubiKey** or **Google Titan Key** for the highest level of security.

---

## **Why Did GitHub Make MFA Mandatory?**
- In **2023**, GitHub made MFA mandatory to:
  - Protect open-source projects and repositories.
  - Prevent account takeovers and supply chain attacks.
- GitHub is critical for the global developer community, and securing it is essential.

---

## **Benefits of MFA**
1. **Enhanced Security**: Protects your account from unauthorized access.
2. **Peace of Mind**: Even if your password is compromised, your account stays safe.
3. **Safeguard Your Projects**: Keeps your repositories secure and prevents malicious code injections.

---

## **How MFA Works – A Simple Example**
Think of your GitHub account as your house:
- Your password is like the key to your house.
- MFA is like adding a **fingerprint scanner** or an **extra lock**. Even if someone has your key (password), they can’t get in without the second layer of security.

---

## **Conclusion**
- Setting up MFA is quick and easy, and GitHub provides multiple options to suit everyone.
- It’s a small step for you but makes a big difference in protecting your code and the developer community.

---

### **Next Steps**
1. Enable MFA on your GitHub account today.
2. Choose the method that works best for you:
   - Authenticator App
   - SMS
   - Hardware Security Key
3. Stay secure and keep your projects safe!

## Preparing Your Working Directory

To set up your working directory, navigate to the **Desktop** folder by running the following commands in the terminal:

```bash
cd       # Navigate to your home directory
cd Desktop   # Change directory to the Desktop folder
```

 

### **What is Version Control, and Why Should I Use It?**

- **Version Control** is a system that tracks changes to your files over time.  
- It allows you to:
  1. **Keep a history** of all changes.
  2. **Undo mistakes** by restoring earlier versions.
  3. **Collaborate** effectively with others without overwriting each other's work.

---





# Explanation with an Example

### **Imagine This Scenario:**
- You’re working on a recipe with your friend.  
- You both make changes to the recipe at the same time. Without version control:
  1. One person’s changes might overwrite the other’s work.
  2. It’s hard to keep track of who changed what and when.
  3. If something goes wrong, there’s no way to go back to an earlier version.

### **How Version Control Solves This:**
1. Each person works on their own copy of the recipe.
2. Changes are **tracked** and stored in a central repository.
3. You can:
   - See a detailed **history** of changes.
   - **Merge** changes from both copies.
   - **Revert** to an earlier version if needed.

---

# Benefits of Version Control

1. **Collaboration**: Multiple people can work on the same project without conflicts.
2. **History Tracking**: You know who made what changes and when.
3. **Backup**: All your work is saved in one secure location.

---


 ##⚙️ Setting Up Git:

### ** How do I get set up to use Git? **
When using Git for the first time on a computer, some configurations are necessary:


Below are a few examples of configurations we will set as we get started with Git:

    our name and email address,
    what our preferred text editor is,
    and that we want to use these settings globally (i.e. for every project).



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
