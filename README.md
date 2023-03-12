# Lab Report 4
_David Sanchez, d4sanchez@ucsd.edu, A16854510_

<br>

## Step 1: (setup) Fork the repository

![Image](lab7report/fork.png)

> Forked the repository from the professor's repository page for Lab 7.  Pressed the fork button in the upper right corner of the page.

![Image](lab7report/forkafter.png)

> Successfully forked his repository and was prompted to create my own repository for Lab 7.

<br>

## Step 2: Log into ieng6

![Image](lab7report/login.png)

> Prior to this, created a new Bash terminal in the bottom right corner of my Visual Studio code editor.  Typed in: 
> `ssh cs15lwi23auh@ieng6.ucsd.edu`, `<enter>` 
> Following the implementation of my SSH key through my personal laptop to my server account, my password was no longer needed to log in.

![Image](lab7report/loginafter.png)

> Successfully logged into the UCSD ieng6 server.

<br>

## Step 3: Cloning my fork of the repository from my Github account

![Image](lab7report/gitclone.png)

> Used `git clone git@github.com:davchez/lab7.git`, `<enter>` to clone the fork of my new Lab 7 repository and used the repository-specific SSH link (not HTTPS link) to ensure that all future adds, commits, and pushes were successful in the future.

![Image](lab7report/gitcloneafter.png)

> Successfully cloned my repository into my server user directory for use.

<br>

## Step 4: Run the tests, demostrating that they fail

![Image](lab7report/junitfail.png)

> Typed in: <br>
> `cd lab 7`, `<enter>`. <br>
> `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java`, `<enter>` <br>
> `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests`, `<enter>` <br>
> ListExamplesTester detected a time-out error on one of its tests, implying that there exists some form of forever loop or unbreakable code in ListExamples.

<br>

## Step 5: Edit the code to fix the failing test

![Image](lab7report/nano.png)

> Typed in `nano ListExamples.java`, `<enter>` to pull up the terminal editing screen for the Java file.

![Image](lab7report/nanoafter.png)

> (Actual keys pressed below.)  Accessed the nano terminal editing screen to change line 43 from "index1 += 1" to "index2 += 1", which was the cause of the time-out error on the JUnit test.

> _Keys pressed:_ `<ctrl> + <W>`, typed in `index1 += 1`, `<enter>`, pressed `<right>` 14 times, <backspace>`

![Image](lab7report/nanoedit.png)

> Edit shown above.

![Image](lab7report/nanosave.png)

> (Actual keys pressed below).  Pressed `<ctrl> + <O>` to save my changes and to ensure that it was being saved to the right filename.

> _Keys pressed:_ `<ctrl> + <O>, <enter>`

![Image](lab7report/nanoexit.png)

> (Actual keys pressed below).  Pressed ctrl-X to exit the nano editing screen.

> _Keys pressed:_ `<ctrl> + <X>`

<br>

## Step 6: Run the tests, demonstrating that they now succeed

![Image](lab7report/recompile.png)

> (Actual keys pressed below).  Pressed up seven times due to incorrect inputs/pastes prior to this screenshot, then accessed the JUnit compile command.  Pressed up seven times again to access the JUnit run command on the JUnit file ListExamplesTests, which ran successfully and without any errors.

> _Keys pressed:_ `<up><up><up><up><up><up><up><enter>, <up><up><up><up><up><up><up><enter>`

<br>

## Step 7: Committing and pushing the resulting change to my Github account

![Image](lab7report/gitaddcommit.png)

> Typed the `git add *` command to add all existing and new changes to the next commit.  Typed the `git commit -m` command with an update message after `-m`.  Indirectly, this avoids forcing the Visual Studio code editor into the VIM interface, which is ultimately not that easy to work with.  

![Image](lab7report/gitpush.png)

> Typed the `git push` command to push all committed changes to the GitHub repository.

![Image](lab7report/gitresult.png)

> Successfully updated necessary .java files and added new .class files from the compilation in Bash.
