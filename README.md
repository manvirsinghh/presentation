 # 📝 Daily Live Report (6 Months)
 # 📊 GitHub Workshop Report

📅 Date: 15/01/2025

⏰ Start Time: 7:00 PM

⏳ End Time: 9:00 PM

---

 ### 🔍 Learnings from the Workshop:

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

![image](https://github.com/user-attachments/assets/42763daf-897c-4e12-a228-1a6d10de6f22)

The commands themselves don't produce any output to the terminal by default if they are successful.
To verify that the configuration was set correctly, you can use the following command:
``` Bash

git config --list
```
---

This command will display all your current Git configuration settings, including your username and email. 

**The Git username and email used for commits can be different from your account credentials on platforms like GitHub**

Here's why:

   **Git Configuration is Local**: The username and email you set in your local Git configuration are primarily used to identify you as the author of commits within your local repository and when pushing changes to remote repositories.
    
   **Platform Accounts are for Authentication**: Your account credentials on platforms like GitHub are used for authentication and authorization – to access and manage repositories on those platforms.

In summary:

    You can use any username and email for your Git configuration.
    These details are primarily used for tracking changes within your local repository and attributing commits to you.
    Your platform account credentials are used for accessing and managing repositories on those platforms.

 No we can not include spaces in your Git username

We  can use Git without GitHub.  
GitHub makes it easier to use Git by providing a central location for your projects, facilitating collaboration, and offering additional features
Git Help and Manual:

```bash
$ git config -h
$ git config --help
```

📂 Creating a Repository:
Once Git is configured, we can start using it.

First, let’s create a new directory in the Desktop folder for our work and then change the current working directory to the newly created one:
Let see i have this created this directory/folder in desktop

![image](https://github.com/user-attachments/assets/73147de6-0905-4a14-a54f-13a691cc3a4f)

Then we tell Git to make recipes a repository -- a place where Git can store versions of our files:

![image](https://github.com/user-attachments/assets/30856119-f215-4df3-ae6f-b47c92793dde)

note that the creation of the recipes directory and its initialization as a repository are completely separate processes.
If we use ls to show the directory’s contents, it appears that nothing has changed:
![image](https://github.com/user-attachments/assets/f42ea613-0fe3-478b-9e7f-b6bc6dabf8f3)

But if we add the -a flag to show everything, we can see that Git has created a hidden directory within recipes called .git:

![image](https://github.com/user-attachments/assets/0d69dc35-0b83-455c-9ae0-4ce36a84301b)


Git uses this special subdirectory to store all the information about the project, including the tracked files and sub-directories located within the project’s directory. If we ever delete the .git subdirectory, we will lose the project’s history.

**We can now start using one of the most important git commands, which is particularly helpful to beginners. git status tells us the status of our project, and better, a list of changes in the project and options on what to do with those changes. We can use it as often as we want, whenever we want to understand what is going on**

![image](https://github.com/user-attachments/assets/99790a33-7a57-43d9-91df-61e3abab18c0)

**Tracking Changes**

   ## 1.How do I record changes in Git?
   ## 2.How do I check the status of my version control repository?
   ## 3.How do I record notes about what changes I made and why?
   
   First let’s make sure we’re still in the right directory. You should be in the recipes directory.

![image](https://github.com/user-attachments/assets/5bd6283f-8f8f-444f-8515-4819f3a92a52)

Let’s create a file called guacamole.md that contains the basic structure of a recipe. We’ll use nano to edit the file; you can use whatever editor you like. 


   ![image](https://github.com/user-attachments/assets/74d98bb4-d989-401a-a3c1-714172d6c32f)

This will open the editor like this 

![image](https://github.com/user-attachments/assets/a2fb9d17-b2f6-4a03-b9cb-e8d6a2720677)


Type the text below into the guacamole.md file:
![image](https://github.com/user-attachments/assets/e80b7e17-c33e-4eeb-93b2-11652a5d9ade)

Save the file  by pressing ctrl+O and press enter and exit your editor using ctrl+X. Next, let’s verify that the file was properly created by running the list command (ls):

![image](https://github.com/user-attachments/assets/408372d9-1db6-47fb-8be7-adb6e99d1177)

guacamole.md contains three lines, which we can see by running:

![image](https://github.com/user-attachments/assets/0dbbc47b-7f05-47e8-8677-038a029c1e07)


If we check the status of our project again, Git tells us that it’s noticed the new file:


![image](https://github.com/user-attachments/assets/4df05d4d-391c-477b-b773-3663f8a2e1ba)


The “untracked files” message means that there’s a file in the directory that Git isn’t keeping track of. We can tell Git to track a file using git add:


![image](https://github.com/user-attachments/assets/73465623-ed2b-4b1e-b033-a8e86e3f74eb)


and then check that the right thing happened:


![image](https://github.com/user-attachments/assets/3b4b7555-a473-4d1a-ab77-fffad722a7c1)


Git now knows that it’s supposed to keep track of guacamole.md, but it hasn’t recorded these changes as a commit yet. To get it to do that, we need to run one more command:
![image](https://github.com/user-attachments/assets/f4c642c9-4e42-40fb-881a-c82f380e1c90)


When we run git commit, Git takes everything we have told it to save by using git add and stores a copy permanently inside the special .git directory. This permanent copy is called a commit (or revision) and its short identifier is f22b25e. Your commit may have another identifier.

We use the -m flag (for “message”) to record a short, descriptive, and specific comment that will help us remember later on what we did and why. If we just run git commit without the -m option, Git will launch nano (or whatever other editor we configured as core.editor) so that we can write a longer message.


If we run git status now:
![image](https://github.com/user-attachments/assets/cd51e047-d1d4-4af4-943a-ac7fc2f40b75)




it tells us everything is up to date. If we want to know what we’ve done recently, we can ask Git to show us the project’s history using git log:

![image](https://github.com/user-attachments/assets/6f6d7ba5-0f0a-417d-a377-684f52559271)

git log lists all commits made to a repository in reverse chronological order. The listing for each commit includes the commit’s full identifier (which starts with the same characters as the short identifier printed by the git commit command earlier), the commit’s author, when it was created, and the log message Git was given when the commit was created.




**Where Are My Changes?**

If we run ls at this point, we will still see just one file called guacamole.md. That’s because Git saves information about files’ history in the special .git directory mentioned earlier so that our filesystem doesn’t become cluttered (and so that we can’t accidentally edit or delete an old version).

Now suppose we adds more information to the file. (Again, we’ll edit with nano and then cat the file to show its contents)

![image](https://github.com/user-attachments/assets/8c9c2e06-f13b-43bb-96c3-efff54123cce)

now press enter to go nano editor to add some more contacts in file we have created earlier 
![image](https://github.com/user-attachments/assets/c3c611a5-6dc4-4cc7-8356-03245de38a40)


When we run git status now, it tells us that a file it already knows about has been modified


![image](https://github.com/user-attachments/assets/50f2f537-36a3-4721-bc32-ee574aa9256e)


The last line is the key phrase: “no changes added to commit”. We have changed this file, but we haven’t told Git we will want to save those changes (which we do with git add) nor have we saved them (which we do with git commit). So let’s do that now. It is good practice to always review our changes before saving them. We do this using git diff. This shows us the differences between the current state of the file and the most recently saved version:


![image](https://github.com/user-attachments/assets/ac027025-e8fe-4f38-a0a2-8aa14a15402a)




    The first line tells us that Git is producing output similar to the Unix diff command comparing the old and new versions of the file.
    The second line tells exactly which versions of the file Git is comparing; b5426e1 and c42c916 are unique computer-generated labels for those versions.
    The third and fourth lines once again show the name of the file being changed.
    The remaining lines are the most interesting, they show us the actual differences and the lines on which they occur. In particular, the + marker in the first column shows where we added a line.

After reviewing our change, it’s time to commit it:
![image](https://github.com/user-attachments/assets/d43dfe2c-f607-4fec-ac15-bc6384519224)


###### Whoops: Git won’t commit because we didn’t use git add first. Let’s fix that:

![image](https://github.com/user-attachments/assets/581d45b7-06d5-41f3-8d78-0d1fb05e6648)

Git insists that we add files to the set we want to commit before actually committing anything. This allows us to commit our changes in stages and capture changes in logical portions rather than only large batches. 



# Staging Area:

Git takes snapshots of changes over the life of a project. The `git add` command specifies what will go into a snapshot (putting things in the staging area), and `git commit` actually takes the snapshot and makes a permanent record of it (as a commit). If you don't have anything staged when you type `git commit`, Git will prompt you to use `git commit -a` or `git commit --all`. However, it's almost always better to explicitly add things to the staging area, because you might commit changes you forgot you made.

📌 Illustrative Diagram:

![Diagram](https://github.com/user-attachments/assets/639861d6-1306-49ab-aaf7-1a2f81d5fa62)

**Exploring History**


Before we start, let’s make a change to guacamole.md, adding yet another line.


![image](https://github.com/user-attachments/assets/4d112a17-34c1-4b2f-a3bd-6854b35fe827)





![image](https://github.com/user-attachments/assets/086a86dc-6cf6-497d-a703-715ca27ad92e)


Now, let’s see what we get.
![image](https://github.com/user-attachments/assets/e6bf9d49-06a1-497e-a433-82caffb33bf6)



Note that HEAD is the default option for git diff, so omitting it will not change the command’s output at all (give it a try). However, the real power of git diff lies in its ability to compare with previous commits. For example, by adding ~1 (where “~” is “tilde”, pronounced [til-duh]), we can look at the commit before HEAD.


![image](https://github.com/user-attachments/assets/6a14be4d-ec67-4358-b2bc-614385dfb564)





You can check it has same output 
![image](https://github.com/user-attachments/assets/82174314-c702-4eef-8fcd-7f457b512b1f)

**Exploring history**

We can put things back the way they were by using git restore:


![image](https://github.com/user-attachments/assets/c8ecd60f-4292-437a-a77e-3bc37ff229c1)


**Ignoring Things**

###### How can I tell Git to ignore files I don’t want to track?

What if we have files that we do not want Git to track for us, like backup files created by our editor or intermediate files created during data analysis? Let’s create a few dummy files:



![image](https://github.com/user-attachments/assets/06ecdb65-a5bb-402f-a1d8-abfd25ad3819)


and see what Git says:

![image](https://github.com/user-attachments/assets/f451ecf3-b381-428f-9c4d-8875f32f0dbc)

To prevent Git from tracking these files and to avoid unnecessary disk space usage or distractions, you can use a .gitignore file

We do this by creating a file in the root directory of our project called .gitignore:

![image](https://github.com/user-attachments/assets/e78665f9-686d-43d0-a4e9-433af0e266cc)




![image](https://github.com/user-attachments/assets/91841fad-6615-4a29-ab16-cd70c4d7d35d)



These patterns tell Git to ignore any file whose name ends in .png and everything in the receipts directory. (If any of these files were already being tracked, Git would continue to track them.)



   ### Remotes in GitHub


 ##### How do we share my changes with others on the web?


 Let’s start by sharing the changes we’ve made to our current project with the world. To this end we are going to create a remote repository that will be linked to our local repository.



##  1. Create a remote repository:-
Log in to GitHub, then click on the icon in the top right corner to create a new repository called recipes:



 ![image](https://github.com/user-attachments/assets/03c1e97c-82eb-4d33-8b90-0bc8e08af441)



 Name your repository “recipes” and then click “Create Repository”.





 Note: Since this repository will be connected to a local repository, it needs to be empty. Leave “Initialize this repository with a README” unchecked, and keep “None” as options for both “Add .gitignore” and “Add a license.” See the “GitHub License and README files” exercise below for a full explanation of why the repository needs to be empty.
The second step in creating a repository on GitHub: filling out the new repository form to provide the repository name, and specify that neither a readme nor a license should be created


![image](https://github.com/user-attachments/assets/b1877b00-da70-4a38-9434-db240c01c172)



Click on create button to create the repository

As soon as the repository is created, GitHub displays a page with a URL and some information on how to configure your local repository:



![image](https://github.com/user-attachments/assets/7d22e5f2-628a-4c4c-ab48-92287682bdff)








**2. Connect local to remote repository**

Now we connect the two repositories. We do this by making the GitHub repository a remote for the local repository. The home page of the repository on GitHub includes the URL string we need to identify it:


![image](https://github.com/user-attachments/assets/cd3ab4a9-9a52-4867-a7e5-6c6a5e0ec580)



Copy that URL from the browser, go into the local recipes repository, and run this command:


![image](https://github.com/user-attachments/assets/e4072c4d-f472-49cb-9604-0a36c8eb0629)

origin is a local name used to refer to the remote repository. It could be called anything, but origin is a convention that is often used by default in git and GitHub,



We can check that the command has worked by running git remote -v:

![image](https://github.com/user-attachments/assets/a220f413-b9e5-4d02-90e8-3ab0c8097889)


We’ll discuss remotes in more detail further , while talking about how they might be used for collaboration.




 **3) Push local changes to a remote**

 This command will push the changes from our local repository to the repository on GitHub:



 ![image](https://github.com/user-attachments/assets/7e3a6a1e-79aa-46e1-8e17-b657c4b90363)


**Collaborating**


 ###### How can weuse version control to collaborate with other people?

 For the next step, get into pairs. One person will be the “Owner” and the other will be the “Collaborator”. The goal is that the Collaborator add changes into the Owner’s repository. We will switch roles at the end, so both persons will play Owner and Collaborator.



 The Owner needs to give the Collaborator access. In your repository page on GitHub, click the “Settings” button on the right, select “Collaborators”, click “Add people”, and then enter your partner’s username
Here I am owner and sukhlotey is collaborator 

 ![image](https://github.com/user-attachments/assets/2523bb79-0701-41c6-b209-0635dd998e66)


Then add people 

![image](https://github.com/user-attachments/assets/c737220f-30db-4414-9914-050ef14164ba)

i have successfully added the collaborator named sukhlotey



To accept access to the Owner’s repo, the Collaborator needs to go to https://github.com/notifications or check for email notification. Once there he can accept access to the Owner’s repo.

Next, the Collaborator needs to download a copy of the Owner’s repository to her machine. This is called “cloning a repo”.



The Collaborator doesn’t want to overwrite her own version of recipes.git, so needs to clone the Owner’s repository to a different location than her own repository with the same name.



To clone the Owner’s repo into her Desktop folder, the Collaborator enters:

$ git clone git@github.com:username/recipes.git folder name 



**Conflicts**

###### What do I do when my changes conflict with someone else’s?




As soon as people can work in parallel, they’ll likely step on each other’s toes. This will even happen with a single person: if we are working on a piece of software on both our laptop and a server in the lab, we could make different changes to each copy. Version control helps us manage these conflicts by giving us tools to resolve overlapping changes.

**Citation**
A citation is a way to give credit to the original creator of a project or work. On GitHub, it’s a way for others to reference your code or project in their own work, like in research papers.


### *Hosting*
Hosting on GitHub typically refers to making your project or website available online 
1. GitHub Pages

GitHub Pages is a feature that allows you to host a website directly from a GitHub repository. It's mainly used for personal, project, or documentation websites.

    How it works: You create a repository, push your HTML, CSS, and JavaScript files to it, and GitHub hosts it for you.
    Usage:
        Personal site: https://username.github.io
        Project site: https://username.github.io/repository-name

To set up GitHub Pages:

   -  Go to your repository settings.
   -  Scroll down to the GitHub Pages section.
   -  Choose the branch you want to publish (usually main or gh-pages).
   -  Your site will be available at https://username.github.io/repository-name.
