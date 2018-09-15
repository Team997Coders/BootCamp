# Coding Boot Camp

### A Guide For New Developers
### Spartan Robotics, Team 997

---

### Where To Start?
#### Simple: at the beginning.

- Integrated Development Environment (IDE): Microsoft VSCode
- Build Tools: Gradle
- Java Fundamentals
- Source code control (Git)
- WPILIB: Between you and the robot

---

### Introducing Microsoft VSCode

- Lightweight integrated development environment: Code, build, test, debug, blame, and deploy
- Multi-platform: Runs on Windows, Linux, and Mac
- Multi-language: Plugins for C#, C++, Ruby, Java, Python, NodeJS, and many more
- Integration with source code control (we use Github)
- Integrated debugger
- [Download](https://code.visualstudio.com/download) and install from Microsoft

---

### VSCode: What you need to know

- One key combination!
  - Ctrl-Shift-P
  - Remember it, know it, love it!
- Welcome page...go though topics
- Plugins: Makes VSCode work for you
  - You'll need:
    - [Microsoft Java Extension Pack](https://code.visualstudio.com/docs/languages/java#_install-java-extensions)
    - [Git](https://git-scm.com/download) Plugin built in, but Git must be installed
      - [Git Cheatsheet](https://services.github.com/on-demand/downloads/github-git-cheat-sheet.pdf)
    - [WPILib](https://github.com/wpilibsuite/vscode-wpilib/releases) Download and install latest vsix file

---

### VSCode: Required Settings

- Ctrl-Shift-P
- Type settings
- Pick User Settings
- Set auto file save to 'onFocusChange'
- You're welcome!

---

### About Gradle

- General purpose build tool (see [Quickstart](https://docs.gradle.org/current/userguide/tutorial_java_projects.html))
- Useful because building and packaging projects is a pain
- javac, the Java compiler, must be called for every source code file
- Compiled files are then packaged into jar files
- Other steps are usually involed (automated testing, for example)
- Gradle automates this process

---

### Gradle Fundamentals

- Gradle by itelf does not do much
- build.gradle file contains Gradle commands for given directory
- Plugins add the magic
```
apply plugin: 'java'
```
- Tasks are the magic added by the plugin
```
gradle tasks
```
- Dependencies and repo 
---

### About Git

- Source code control system
- Supports tracking code versions in a team environment
- Commits serve a checkpoints for supposedly working code
- Commits are stored locally
- Do small bits of work, make those bits at least compile, and then commit
- A push must be done to get code to central serer
- Branches serve as a base point to work a separate code base

---

### The Git Adventure

- New project requires an initialized local repository (repo)
- New files must be added and then committed to local repo
- You can do this in VSCode, debug pane, type commit message and press Ctrl-Enter
- This DOES NOT push your code to the web (github.com)

---

### Pushing Code to github.com

- You need a Github account and have lead authorize you to Team997Coders
- Create a [personal access token](https://help.github.com/articles/creating-a-personal-access-token-for-the-command-line/)
- Create a new remote repository in github.com
- In root project directory, point to remote repository
```
git remote add origin https://github.com/Team997Coders/<repo name>.git
```
- Enable windows credential manager to store your credentials
```
git config --global credential.helper wincred
```

---

### Pushing Code to github.com (cont)

- Push code to web
```
git push -u origin master
```
- Git will prompt you for username and password
- Use the personal access token for password
- If VSCode continues to nag you for credentials as you use git, you did something wrong
- Committing and pushing can then be done from VSCode menus without using command line
