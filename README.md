# Lesson Plan

## Before we start

- [ ] Have you installed (i) [R](https://cran.rstudio.com), (ii) [RStudio](https://posit.co/download/rstudio-desktop/), and of course (iii) [git](https://git-scm.com) on your machine?
- [ ] Have you installed a bash compatible shell? (Windows only)
    - [Git for windows](https://gitforwindows.org/) Comes pre-installed with Git, often providing all the necessary functionality for the course as the baseline requirement.
    - Rtools shell comes pre-installed with Rtools
    - [Windows Subsystem for Linux (WSL)](https://learn.microsoft.com/en-us/windows/wsl/install) is an Ubuntu bash shell for Windows. Comes pre-installed with htop, apt-get, and make.
- [ ] Are they all updated to their most recent version?
- [ ] Have you already created an account on GitHub and have your password ready?
    - Does your account have a profile picture? Your full name? :eyes:
- [ ] Make sure that some further software is installed
    - Windows
        - Install [Rtools](https://cran.r-project.org/bin/windows/Rtools/)
        - Install [Chocolatey](https://chocolatey.org/)
    - Mac
        - Install [Homebrew](https://brew.sh/)
        - Configure [C++ toolchain](https://github.com/coatless-mac/r-macos-rtools#installer-package-for-macos-r-toolchain-)
    - Linux
      - None :)

## Introductory Resources

> [!NOTE]
> Do not worry, not all of the resources need to be read. The resources have a large overlap, but some people might like one resource more than another (we certainly did observe this among us). Important is, that you get a first overview of what git, GitHub, and the shell are. 

- [Happy Git with R](https://happygitwithr.com/) is a beginner-friendly website that introduces git with R and RStudio
    - In addition, we recommend appendix A which links R, git, and the shell
- GitHub provides a nice [CheatSheet](https://education.github.com/git-cheat-sheet-education.pdf)
- GitLab also provides a nice [CheatSheet](https://about.gitlab.com/images/press/git-cheat-sheet.pdf)
- [TryBash](https://trybash.github.io/) is an interactive course and cheatsheet for basic bash commands
- [Git Gud](https://github.com/benthayer/git-gud) is a Python-based gamified introduction to git
- There's also this [playlist on YouTube](https://www.youtube.com/watch?v=BCQHnlnPusY&list=PLRqwX-V7Uu6ZF9C0YMKuns9sLDzK6zoiV)
- [Code and Data for Social Science](https://web.stanford.edu/~gentzkow/research/CodeAndData.pdf) is a great text that can guide readers into important aspects of coding and data for social sciences
    - Some sections may be more advanced, but the chapter on Version Control will be especially useful for us
- The Holy Grail, i.e. [Grant McDermott's Lecture Notes](https://github.com/uo-ec607/lectures?tab=readme-ov-file) has everything you need and more on Git, the shell, and anything else your mind might think of.
- [My git is now irreversibly messed up](https://ohshitgit.com/)
- Additional Reading
    - [Shell for Novices](https://swcarpentry.github.io/shell-novice/)
    - [Data Science at the Command Line](https://datascienceatthecommandline.com/)

## Shell

> [!NOTE]
> A CheatSheet for bash can be found in the `bash-cheatsheet` folder.

- [ ] opening the shell on Mac, Linux, Windows
    - Use bash or zsh preferably
    - Windows may prefer [Windows Subsystem for Linux (WSL)](https://learn.microsoft.com/en-us/windows/wsl/install)
        - Is this better than using the shells from git or Rtools? Yes - for certain applications. WSL supports e.g. the native Linux package managers and provides an overall more seamless portal to Linux.
        - WSL is like having your own Ubuntu terminal in RStudio without having to install Linux
        - However, for working with git and performing simple operations, the shells from git or Rtools are plenty sufficient
- [ ] Introductory definitions
    - What do all the weird symbols mean? (~ or $ or *)
- [ ] current working directory
- [ ] navigating directories
- [ ] creating folders
- [ ] deleting folders and files
- [ ] moving folders and files
- [ ] [htop](https://htop.dev/) and process viewers
- [ ] installing software using brew (Mac), apt (Ubuntu), Chocolatey/Winget (Windows)
<!-- - [ ] My very first shell script (Or, how to use Julia, C++, and Python in dsri) -->

## Git

- [ ] What is a git folder? 
- [ ] how to initialise a new git folder? 
- [ ] gitignore
- [ ] making changes
- [ ] staging / unstaging changes 
- [ ] committing 
- [ ] branches/forks
- [ ] going back in history (various ways)
- [ ] keeping an overview with gitk


## GitHub
- [ ] logging in
- [ ] making a new repository
- [ ] private / public repos
- [ ] becoming a contributer (add them to this repo so that we can keep having all course notes in this repository)
- [ ] adding remote
- [ ] SSH
- [ ] adding a README
    - [Markdown basics](https://www.markdownguide.org/)
- [ ] pushing / pulling
- [ ] pull requests
- [ ] [Github Issues](https://docs.github.com/en/issues/tracking-your-work-with-issues/about-issues)
- [ ] merge conflicts
- [ ] continuous integration (??) --> standard when developing R and Julia packages but more complicated

## Git, Github, and RProjects
- [ ] How to connect Git/Github with RStudio Projects
- [ ] Cloning an existing GitHub repository
- [ ] Uploading an existing RProject to GitHub
