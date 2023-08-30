<!-- 
<img width="400" src="assets/img/logo-git-github.png"> -->

# Git Milestones




## Instructions

1. Review sections 1-4 (Introduction, CLI Tutorial, Install, Git Tutorial) of [Git & Github](https://docs.google.com/presentation/d/1vtK6LoqwF4rQQZZy-ovuEgsYUwwMRXsqDVMOjAPSBt0/edit#slide=id.p)
1. Complete each task below, creating files and adding content inside the [Completions](#completions) table when prompted: ✏️
1. After you finish, celebrate your Git proficiency! 🙌

#### Notes...

- **RTM** - Sometimes I give the command you need and sometimes you have to read the documentation to find it.
- **Details** - Follow the instructions.
- **Classes** - This milestone is made to use with multiple classes; insert your own class name where you see `<your-class-name-here>` (e.g. `critical-web-design`)





## Part 1 – Git Basics


### 1-1 Markdown

Markdown is a lightweight markup language used to create rich text.

- It has a [simple syntax](https://www.markdownguide.org/cheat-sheet/) similar to [HTML](https://en.wikipedia.org/wiki/Markdown#Example)
- It is the standard language for formatting README files (what you are currently viewing!)
- Files use the `.md` extension and can be edited with any plain text editor (e.g. VS Code).
- Preview using the VS Code or the [Markdown Viewer](https://chrome.google.com/webstore/detail/markdown-viewer/ckkdlimhmcjmikdlpkmbgfkaikojcbjk/related?hl=en) 

Markdown | HTML | Rendered Output
--- | --- | ---
`[link](https://davidson.edu)` | `<a href="https://davidson.edu">link</a>` | [link](https://davidson.edu)
`**bold text**` | `<b>bold text</b>` | **bold text**
`*italicized text*` | `<i>italicized text</i>` | *italicized text*
<code>\`code`</code> | `<code>code</code>` | `code`
`![text](assets/img/icon.png)` | `<img alt="text" src="assets/img/icon.png">` | ![text](assets/img/icon.png)

**Now you know basic Markdown!** 🎉  The following instructions will help you learn Git, editing this `.md` file in the process. Feel free to check your syntax in the [github markdown cheatsheet](reference-sheets/github-markdown-cheatsheet.pdf).

Other Markdown tools

- [Paste (RTF or rendered HTML) to Markdown](https://euangoddard.github.io/clipboard2markdown/)
- [HTML to Markdown](https://codebeautify.org/html-to-markdown)


---

### 1-2 Fork this repository
Create a Github account and make your first commit on Github.com

1. [Create a Github account](https://github.com/join)
1. Fork this [learn-git-milestones](https://github.com/omundy/learn-git-milestones) repository (click the Fork button, top right).
1. ✏️ Edit this `README.md` file (click the pencil icon on the Github.com page) and add your *1st* favorite emoji to the [Completions](#completions) table, in the **Completed** column in appropriate row in the [completions](#completions), below.
1. Commit changes to README.md to the `main` branch with the message `commit #1 from Github.com`.
1. ✏️ Use [Markdown documentation](https://guides.github.com/features/mastering-markdown/) to add a link in [completions](#completions). The link text should be the same as the commit message, and the url should point to the Github.com page showing the above commit.
1. ✏️ Tables can be a little tricky in Markdown. Find a good link explaining how to use markdown tables. Paste the link in the [Completions](#completions) table.
1. View the commit history and confirm your edits


---

### 1-3 Git Installation

Install your development environment

1. Complete the [command line crash course](https://github.com/omundy/learn-computing/blob/main/topics-command-line.md#crash-course)
1. Install Git on your machine ([via](https://gist.github.com/derhuerst/1b15ff4652a867391f03))

**Windows**
1. Install [Git for Windows](https://gitforwindows.org/) (includes [Git BASH](https://www.atlassian.com/git/tutorials/git-bash), its own version of the bash shell)

**Mac**
1. Install the [homebrew package manager](https://brew.sh/) (confirm "yes" if asked to install *Command Line Developer Tools*)
1. Install git using Homebrew `brew install git` (unless you are [upgrading](https://ajahne.github.io/blog/tools/2018/06/11/how-to-upgrade-git-mac.html)?)
<!-- 1. Set your default shell to bash `chsh -s /bin/bash` - You'll be prompted to type a password. The command line doesn't give you feedback that you're typing. Just type your password and hit enter. Backspace a lot if you make a mistake. -->


---

### 1-4 Configure Git

1. When you first install or start using Git, verify it is installed by typing `git` on the command line and hitting enter. This displays a help file with a list of possible commands.
 	- ✏️ What does `log` do? Add your answer to [completions](#completions).
2. Then you should update the configuration. Add your name and email (replace with your information and press return after each line)

```bash
git config --global user.name "Jane Doe"
git config --global user.email janedoe@example.com
```

3. Set the [default branch to main](https://www.theserverside.com/feature/Why-GitHub-renamed-its-master-branch-to-main)

```bash
git config --global init.defaultBranch main
```

4. Set pull to merge ([not rebase](https://stackoverflow.com/a/36587353/441878))

```bash
git config --global pull.rebase false
```

5. Confirm your global settings worked with either of these [1](https://stackoverflow.com/a/46986031/441878)

```bash
# show contents of global config
cat ~/.gitconfig
# or show settings and location of each config file (system, global, local)
git config --list --show-origin
```






## Part 2 – Basic Git workflows

Perform a basic Git workflow using Github.com, the command line, Github Desktop, and Git in a preferred text editor (e.g. VS Code). These four different interfaces will give you practice and help you understand Git better. You've already forked and made a commit on Github.com so let's move to Github Desktop ...


---

### 2-1 Using Github Desktop

#### Setup

1. Install a [source-code editor](https://en.wikipedia.org/wiki/Source-code_editor) (e.g. [VS Code](https://code.visualstudio.com/)) on your machine 
1. In VS Code connect your Github account
1. Install [Github Desktop](https://desktop.github.com/)
1. Connect your Github account in Github Desktop

#### Clone the fork

1. In Github Desktop, clone the fork (you made above) [learn-git-milestones](https://github.com/omundy/learn-git-milestones) ...
1. File > Clone Repository > Github.com and select it ...
1. Local Path: Click "Choose" and add a new folder on your computer. This will be the base folder for your work in this class (e.g. `critical-web-design`, `game-development` )
1. Click "Clone" to make a local copy

#### Open in VS COde

1. Open the repo in VS Code: Repository > Open in VS Code (see preferences to change your editor)
1. ✏️ In VS Code, edit this README file and add your *2nd* favorite emoji to [completions](#completions).
1. In Github Desktop, view/confirm your edits to the README file on the Changes tab
1. ✏️ Commit your changes directly to the main branch with the message `commit #2 from Github Desktop`. 
1. Find a link to the above commit on Github.com and use VS Code to add it to [completions](#completions). Commit your change.
1. Click Push origin to push your new commit to remote repo
1. Confirm the changes to the README file were pushed: Choose Repository > View on Github
1. Click on the README file and then click on History to see the history of this file


---

### 2-2 Use Git on the Command line 

You should have a basic familiarity with the command line interface (CLI) to install Git. Some folks use the CLI as their default tool for editing and publishing source code, but Github Desktop makes it much easier.

#### Setup

1. If you haven't yet, complete the [command line crash course](https://github.com/omundy/learn-computing/blob/main/topics-command-line.md#crash-course)
1. In Github Desktop, with the [learn-git-milestones](https://github.com/omundy/learn-git-milestones) repo you cloned above selected, click Repository > Open in Terminal ("Bash" in Windows?)

#### Use the CLI to navigate directories

1. List files in this directory: `ls`
1. List files in this directory, including hidden: `ls -la`
1. Confirm the existence of the `.git` directory (where Git versions and config are stored)
1. View your current directory and copy the full path: `pwd`
1. Open this README file in VS Code and paste that path in [completions](#completions).

#### Use Git on the CLI

1. [Confirm](https://docs.github.com/en/github/using-git/setting-your-username-in-git) your name and email is correct in the Git config
1. View the status of your repo: `git status`
1. View the changed files of your repo: `git diff`
1. Add all changed files to the staging area `git add .`
1. View the status of your repo `git status` to confirm it has been staged
1. ✏️ Commit your changes with the message `commit #3 from CLI`. Add a link to this commit to [completions](#completions).
1. Use `git push` to [push those changes to your remote repo](https://docs.github.com/en/github/using-git/pushing-commits-to-a-remote-repository)



You've used most of these already through a GUI (e.g. `git status`, `git add`, `git commit`, `git push`) ...




---

### 2-3 Git in VS Code

1. In Github Desktop, open this repo [learn-git-milestones](https://github.com/omundy/learn-git-milestones) in VS Code: Repository > Open in VS Code
1. ✏️ In VS Code, edit this README file and add your *3rd* favorite emoji to [completions](#completions).
1. ✏️ Create a new file `hello.txt`, add some text and save it.
1. Display the Git panel (click the small Git button at the bottom right).
1. Select on your file(s) in Unstaged changes and confirm your changes match what you expect to see
1. Double click on each file with changes to stage them
1. ✏️ Commit your changes directly to the main branch with the message `commit #4 from VS Code`. Add a link to this commit to [completions](#completions).


<img src="assets/img/editor-git-menu-vs-code.png" width="400">



## Part 3 – Create a new repository

### 3-1 Create a new git repository from scratch

1. ✏️ In Github Desktop, create a new repository with the name: `first-website`
1. Make sure the repository is public *not private* 
1. Local Path: Click "Choose" and create a new folder `first-website` inside the `<your-class-name-here>` folder you made above
1. Click Create Repository
1. This should now be your class folder's directory structure.

```html
<your-class-name-here>
|-- first-website
|-- learn-git-milestones
```

1. Open your new repository in VS Code (with Github Desktop or drag the `first-website` project folder onto the VS Code icon in your dock)
1. ✏️ Add a README file: `README.md`
1. ✏️ In the README write your name and the date
1. ✏️ Use some [Markdown tags](https://guides.github.com/pdfs/markdown-cheatsheet-online.pdf)
1. ✏️ Commit your changes and add a link to this repo to [completions](#completions).




## Part 4 – Publish a web site with Github Pages

[Github Pages](https://pages.github.com/) is a free and easy way to host a website from your repository. 

1. ✏️ Create a file called `index.html` in your new repo and add the following code

```html
<!DOCTYPE html>
<html>
<head>
<title>My first github.io website</title>
</head>
<body>

<h1>Hello world!</h1>
<p>🙌</p>

</body>
</html>
```

1. On Github.com, go to your repo > Settings > Pages
1. Select the main branch source and click save
1. Do not use a theme. Start from scratch
1. Visit your project site at http://*username*.github.io/first-website
1. Update your project, push a new commit, and confirm your updates (note: [deployments](https://github.com/omundy/learn-git-milestones/deployments/github-pages) sometimes take a bit)
1. ✏️ Paste this link to [completions](#completions).






## Part 5 – Turn in this Assignment

Now that we have basic Git commands out of the way use Git to create and turn in your assignment ...

1. Complete all of the items on this README, making sure all the rows in the "Completed" column contain your information below.
1. Test your file(s) in a web browser
1. Commit and push the files to Github
1. Paste the github.io link into the appropriate Moodle forum



<!-- 
## Git Advanced

That is all that is required for this milestone. See the `ADVANCED.md` file if you would like to continue learning Git.
 -->




## Completions

Item # | Description | Completed
--- | --- | ---
1a | 1st Favorite emoji | 🙌
1b | Link to `commit #1 from Github.com` | [commit #1 from Github.com](https://github.com/omundy/learn-git-milestones/compare/main...yodering:learn-git-milestones:main)
1c | Link to markdown tables docs | https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/organizing-information-with-tables
1d | What does `log` do? |
2a | 2nd Favorite emoji |
2b | Link to `commit #2 from Github Desktop` |
2c | Full path to your working directory |
2d | Link to `commit #3 from CLI` |
2e | 3rd Favorite emoji |
2f | Link to `commit #4 from VS Code` |
3a | Link to `first-website` github.com repo page |
4a | Link to `first-website` github.io "project site" |





## Resources

Here are some popular tutorials/guides. You should **still look for other ones that you might like better**!

- The class [Git & Github lectures](https://docs.google.com/presentation/d/1vtK6LoqwF4rQQZZy-ovuEgsYUwwMRXsqDVMOjAPSBt0/edit#slide=id.p)
- [Github Desktop Documentation](https://docs.github.com/en/desktop)
- Github Cheatsheet [HTML](https://github.github.com/training-kit/downloads/github-git-cheat-sheet/) and [PDF](https://github.github.com/training-kit/downloads/github-git-cheat-sheet.pdf)
- [Github Learning Lab](https://lab.github.com/) which contains tutorials like [Introduction to Github](https://lab.github.com/githubtraining/introduction-to-github) and others
- View forks of this repo http://gitpop2.herokuapp.com/omundy/learn-git-milestones


## Credits

Thanks to [Jesse Farmer](https://github.com/jfarmer) for inspiring this milestone assignment.
