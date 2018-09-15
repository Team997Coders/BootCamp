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
- Plugins
  - Makes VSCode work for you
  - You'll need:
    - [Microsoft Java Extension Pack](https://code.visualstudio.com/docs/languages/java#_install-java-extensions)
    - [Git](https://git-scm.com/download) Plugin built in, but Git must be installed
      - [Git Cheatsheet](https://services.github.com/on-demand/downloads/github-git-cheat-sheet.pdf)

---

### The Git Adventure

- New project requires an initialized local repository (repo)
- New files must be added and then committed to local repo
- You can do this in VSCode, debug pane, type commit message and press ctrl-enter
- This DOES NOT push your code to the web (github.com)

### Pushing Code to github.com

- You need a Github account and have lead authorize you to Team997Coders
- Create a [personal access token](https://help.github.com/articles/creating-a-personal-access-token-for-the-command-line/)
- In root project directory, 
- Enable windows credential manager to store your credentials
```
git config --global credential.helper wincred
```
