# IDEA lab Github and Git tutorial

**Table of Contents**
1. [Intro](#intro)
1. [Get started](#get-started)
1. [best practices **IMPORTANT**](#best-practices)
1. [more info](#info)

**What is git?** <a name="intro"></a>

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

**Get started with github** <a name="get-started"></a>

In the following section we will cover the steps to begin uploading your code to our lab's GitHub Organization.

1. **Create a personal GitHub account - [GitHub - create an account](https://docs.github.com/en/get-started/start-your-journey/creating-an-account-on-github) :** This account does not have to be with your school email. Any github account will work, so if you already have one you can skip this step. 

1. **Contact an organization admin about getting an invite to the organization:** You may contact Daniel either by email (dj21@illinois.edu) or through slack, and provide your github email and username, and I will send you an invitation to the organization. (To view our organization visit: https://github.com/UIUC-CEE-IDEA-LAB)

1. **Add your code [(read the docs)](https://docs.github.com/en/migrations/importing-source-code/using-the-command-line-to-import-source-code/about-source-code-imports-using-the-command-line) :** If you already have a personal GitHub repository see step 4, if you only have local code see step 5. If you don't have any code yet, then make a local folder where you would like to store your code then proceed to step 5. 

4. **Importing code from a personal source control repository (must be accessible online) [(read the docs)](https://docs.github.com/en/migrations/importing-source-code/using-github-importer/about-github-importer) :** Go to our organization home > repositories > create new repository; Then select import repository at the top. Or simply visit this link [Import repository](https://github.com/new/import). Follow the prompts to import your repository but change the owner from your personal account to UIUC-CEE-IDEA-LAB (if you don't see the option to select our organization contact an organization admin). You can make the repository public or private depending on your needs. When you work on your local code again, ensure that your remote branch is now pointing to the organization's repository, and not your personal (previous) repository. This can be done with the command `git remote add origin REMOTE_URL`, if you would like to abandon your previous repo you may remove the pointer to that repository using `git remote show` to list all your remote repos, find the name of your old remote repo, then do `git remote remove NAME_OF_REMOTE`

5. **Importing local code with or without source control [(read the docs)](https://docs.github.com/en/migrations/importing-source-code/using-the-command-line-to-import-source-code/adding-locally-hosted-code-to-github) :** Ensure all of your code is inside a project folder, then open this folder using vscode. On VSCode you may initialize a git repository by opening the source control tab *ctrl+shift+G*. Next go to our organization page on GitHub, go to home > repositories > create new repository. or simply visit this link - [create new repository](https://github.com/organizations/UIUC-CEE-IDEA-LAB/repositories/new); if you are unable to create a new repository contact an organization admin. Follow the prompt to create a new repository. It is good practice to name the repository the same name as your local project folder. Ensure that the owner is UIUC-CEE-IDEA-LAB. The repository can be public or private depending on your needs. Navigate into your newly created repository and select the green button "code", then copy the https link. Next, navigate to vscode and open the source control panel, click on the three dots near the top: ... > remote > add remote. This will prompt you to provide the url, as well as the name for your remote. The standard name is either "origin" or "main". Once this is done you must stage all your changes, make your first commit, and push to remote. If you run into issues with any step contact Daniel.

**Best Practices** <a name="best-practices"></a>

* *IMPORTANT* Ensure that there is no sensitive information in your codebase before commiting any changes to git (it will be much harder to remove afterwards). For example usernames, passwords, API keys, etc. If such information is required in a codebase, you should include that information in a separate file such as a config.json that is ignored by git using a .gitignore file, or set the information as environment variables on your machine. For more information on .gitignore see the following tutorial: [git docs - ignoring files](https://git-scm.com/book/en/v2/Git-Basics-Recording-Changes-to-the-Repository#_ignoring)

* For public repositories, it is good to include a README.md file containing information about the project, how to contribute, how to install any dependencies, how to run scripts, etc.

* When publishing code it is good to think about portability wherever it is possible. For example, using libraries such as PathLib in python instead of hard coding directories will avoid file system incompatibility issues. Another example is to use relative paths where possible since the working directory might not be the same in every machine.

* Keep your repository clean of cache files, compiled/built artifacts, or other clutter that can easily be recreated by cloning the repository. This can be done using a .gitignore file. See the link above for more information on ignoring files.

**more info** <a name="info"></a>

* read the docs on github organizations: [github.com](https://docs.github.com/en/organizations)

* full tutorial on git CLI: [Git Tutorial for Beginners: Learn Git in 1 Hour](https://youtu.be/8JJ101D3knE?si=8uyuU-zmjU5BzqkX)
