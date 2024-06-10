# IDEA lab Github and Git tutorial

**What is git?** 

Basic intro to git and git commands:
[YouTube - How Git Works: Explained in 4 Minutes](https://youtu.be/e9lnsKot_SQ?si=-Lz8TeJI4SzPO6zZ)

**What is github?** 

A cloud based, "free", server for storing git repositories.

**How do I use it?** 

There are many ways of using git and github. My (Daniel's) personal favorite is using a combination of VSCode's GUI and the CLI. But really I just use the CLI to clone the repository and for all other purposes I usually use the GUI. However there are many other GUI options out there, and they all just make calls to git commands, so learning the CLI method first is a good place to start.

If your prefered IDE is VSCode, then you have the git GUI, which can be accessed with *ctrl+shift+G*. Or by navigating to the primary sidebar "source control" tab.

Here is a tutorial on familiarizing yourself with VSCode's GUI. The very first video covers most of the day to day use with git:
[Using Git source control in VS code](https://code.visualstudio.com/docs/sourcecontrol/overview)

**Download**

to download VSCode go to the following link: [download visual studio code](https://code.visualstudio.com/download)

for Windows or macOS, go to the following link: [git-scm.com](https://git-scm.com/downloads)

for Ubuntu/Debian Linux, it should already be installed. You can check by opening a terminal and typing the command `which git`. This should return a path to where git is stored on oyur machine, otherwise, you can follow the linux download instructions on the link above. 

**Get started with github**

In the following section we will cover the steps to begin uploading your code to our lab's GitHub Organization.

1. Create a personal GitHub account - [GitHub - create an account](https://docs.github.com/en/get-started/start-your-journey/creating-an-account-on-github) : This account does not have to be with your school email. Any github account will work, so if you already have one you can skip this step. 

1. Contact an organization admin about getting an invite to the organization: You may contact Daniel either by email (dj21@illinois.edu) or through slack, and provide your github email and username, and I will send you an invitation to the organization. (To view our organization visit: https://github.com/UIUC-CEE-IDEA-LAB)

1. Add your code [(read the docs)](https://docs.github.com/en/migrations/importing-source-code/using-the-command-line-to-import-source-code/about-source-code-imports-using-the-command-line): If you already have a personal GitHub repository see step 4, if you only have local code see step 5. If you don't have any code yet, then first make a local folder where you would like to store your code. 

4. Importing code from a personal source control repository (must be accessible online) [(read the docs)](https://docs.github.com/en/migrations/importing-source-code/using-github-importer/about-github-importer): Go to our organization home > repositories > create new repository; Then select import repository at the top. Or simply visit this link [Import repository](https://github.com/new/import). Follow the prompts to import your repository but change the owner from your personal account to UIUC-CEE-IDEA-LAB (if you don't see the option to select our organization contact an organization admin). You can make the repository public or private depending on your needs. When you work on your local code again, ensure that your remote branch is now pointing to the organization's repository, and not your personal (previous) repository.

5. Importing local code with or without source control [(read the docs)](https://docs.github.com/en/migrations/importing-source-code/using-the-command-line-to-import-source-code/adding-locally-hosted-code-to-github) 

**more info**

* read the docs on github organizations: [github.com](https://docs.github.com/en/organizations)

* full tutorial on git CLI: [Git Tutorial for Beginners: Learn Git in 1 Hour](https://youtu.be/8JJ101D3knE?si=8uyuU-zmjU5BzqkX)
