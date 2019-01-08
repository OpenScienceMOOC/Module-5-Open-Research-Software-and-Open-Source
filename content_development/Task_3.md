---
output:
  html_document: default
  pdf_document: default
---

# Task 3: How to integrate Git with R Studio

This task is designed for students and researchers who want to implement a system of version control within a standard R-based workflow. This can be applied to a range of software development, data analysis and project management tasks. Your future research self will thank your for the convenience.

Don't forget you can join in the discussions over at our open [**Slack channel**](https://openmooc-ers-slackin.herokuapp.com/). Please do introduce yourself at #module5opensource, and tell us a bit about who you are, your background, and how you ended up here!

Estimated time to complete: 30 minutes

Estimate time saving once complete: Virtually infinite

**NOTE** A video guide version of this task is now available on [YouTube](https://www.youtube.com/watch?v=Q-6jfjSAspA).

## Table of contents

* [Getting started](#Getting_started)
  * [Git](#Git)
  * [R Studio](#Rstudio)
* [Step one: Download all the things](#one)
* [Step two: Configure Git inside RStudio](#two)
* [Step three: Why did I just do that?](#three)
* [Step four: The perfect marriage between Git and R](#four)
* [Step five: Getting content with content](#five)
* [Step six: A brave commitment](#six)
* [Step seven: PUSH!](#seven)


## Getting started <a name="Getting_started"></a>

Congratulations on making it this far! If you're reading this, you've survived pull requests, web-hooks, and can probably even tell us know what the F in FOSS stands for (*not* Frustration...) Hopefully, you have overcome any scepticism or reluctance towards the benefits of GitHub and Open Source Software, and are ready to take the next step.

Before starting this Task, please make sure you have already completed [Task 1](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/Task_1.md) and [Task 2](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/Task_2.md), so that you are more familiar with GitHub and some standard Open Source practices.

This task will teach you how to integrate the version control software, Git, with the popular coding environment, RStudio. And yes, it is Git as in gif or God, not Jit as in the wrong way of pronouncing things.

If you are one of those researchers who thinks that having code spread across multiple hard-drives that are waiting to break, Dropbox, Google Drive, or any other non-specialist software, this task is just for you. If you have ever experienced the mind-numbing process of having multiple 'final' versions of a paper bouncing between different co-authors, this is also for you.

All of us are guilty of these sorts of things once in a while, but there are ways to do it that are better for you, future you, and those who might benefit from your work.

<br/>

### Getting Git <a name="Git"></a>

So, what is Git, and how is it different to GitHub? Git is a version control system, which enables you to save and track time-stamped copies of your work throughout the development process. It also works with non-code items too, like this MOOC, the majority of which was written in markdown in RStudio, and integrated with a Git/GitHub workflow.

This is important, as all research goes through changes and sometimes we want to know what those things were. Did you delete some text that you now think is important? Version control will save that for you. Did your code work perfectly in the past, but is now buggy beyond belief? Version control. It's a great way to avoid that chaotic state where you have multiple copies of the same file, but without a stupid and annoying file naming convention. `FINAL_Revised_2.2_supervisor_edits_ver1.7_scream.txt` will be a thing of the past.

GitHub is the platform that allows you to seamlessly share code from your workspace (e.g., laptop) to be hosted in an online space. So, sort of like the public interface to GitHub. The advantages of Git/GitHub are:

1. You get to keep copies of all your work through time;
2. You can compare work through different copies through time, which helps to spot bugs or errors;
3. Other people can collaborate openly with your work;
4. You have both a local and an online copy of your work that remain in sync;
5. It is fully transparent as to who made a contribution, why they made it, and when; and
6. You can have multiple people working on the same project at once in parallel.

While this was primarily designed for source code, it should be instantly obvious how this becomes a powerful tool for virtually all research workflows.

<br/>

### RStudio <a name="Rstudio"></a>

RStudio is a popular coding environment for researchers who use the statistical programming language, R. It comes with a text editor, so you don't have to install another and switch between. It also includes a graphical user interface (GUI) to Git and GitHub, which we will be using here.

Isn't it nice when brilliant Open Source tools integrate seamlessly like that. This should help to make your daily use of Git much simpler.

If at any point you need to install new packages for R, simply use the following command:

`install.packages("PACKAGE NAME", dependencies = TRUE)`

Replacing `PACKAGE NAME` with the, er, package name. Some examples you can play with that might come in useful include `knitr`, `devtools` or `ggplot2`.

<br/>

## Step one: Download all the things <a name="one"></a>

1. You should already have a GitHub account by now if you have followed the previous tasks. If not, [sign up here](https://github.com/). Free unlimited repositories for all!
2. Download and install the latest version of [R](https://www.r-project.org/). Also available for [Mac](https://cloud.r-project.org/) and [Linux](https://cloud.r-project.org/bin/linux/).
3. Download and install the latest version of [Rstudio](https://www.rstudio.com/products/rstudio/#Desktop). Oh, hey, looks it Open Source! Swish.
4. Download and install the latest version of [Git](https://gitforwindows.org/). **Make sure to Select “Use Git from the Windows Command Prompt” during installation.**

> **Pro-tip**: To update all of your R packages in one, simply execute the following code `update.packages(ask = FALSE, checkBuilt = TRUE)`

For now, just choose all the usual default options for each install. Depending on which Operating System (e.g., Mac, Windows, Linux), this might be different for each of you. For now, and for the rest of this task, we're going to stick with doing things the easy-ish Windows way (but also provide some instructions for using the command line).

For Linux or Debian users, simply use the following command to install Git:

`sudo apt-get install git-core`

For Mac users, [this link](http://git-scm.com/download/mac), or purchase a new laptop with a different operating system.

If you want, you can also download the [local version of GitHub](https://desktop.github.com/) and use it through the simple GUI. It's available on Windows and Mac and Linux, and can make your life a little easier, especially if you want to use a different platform to RStudio.

> **Pro-tip:** You see when installing Git it says 'Use Git Bash as shell for Git projects?' This is the place where you can use the command-line to access Git from outside of RStudio. It's a powerful beast. Try the following two commands to get started:

`git config --global user.name 'YOUR USERNAME'`
<br/>
`git config --global user.email 'YOUR EMAIL'`
<br/>

## Step two: Configure Git inside RStudio <a name="two"></a>

Right, that's the easy bit done. Next, go into RStudio, and in the tabs at the top go to Go to **Tools > Global Options > Git/SVN**. SVN is just another version control system like Git, and we don't need to worry about that here.

In the place where it says *Git executable*, add the pathway here to the git.exe file that you just downloaded in the previous step. Make sure the box here that says **Enable version control interface for RStudio projects** is ticked. This now has tied version control to future projects in RStudio, to provide a really powerful additional dimension to collaborative or solo work.

<p align="center">
  <img src="https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/images/git_svn.png?raw=true" width="400px"/>
</p>

<p align="center"><i>The Global Options window inside RStudio</i></p>

<br/>

Next, hit the button in this window that says *Create RSA Key*, This is a private key that is used for authentication between different systems, and saves you from having to type in your password over and over. Here, it will pop up a new window with a public key, that you want to copy to your clipboard.

Head over to GitHub, go to your profile settings, and the *SSH and GPG keys* tab. Click *New SSH key*. Here, paste in the key from RStudio, and call it something imaginative like 'RStudio'.

<p align="center">
  <img src="https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/images/ssh_key.png?raw=true" width="800px"/>
</p>

<p align="center"><i>Inside GitHub where you will want to enter the key you just generated in RStudio</i></p>

<br/>

OK, now hold on to your butts, we're going into the command line. Don’t worry if you’ve never used the shell before because it’s quite similar to using R, or any other coding system. The main difference here though is that instead of calling functions like in R, you call commands.

So back in RStudio, go to **Tools > Shell**, and it will open up a command prompt window. If you already played with the Git Bash above, you should have done this step already. Enter the following two commands:

`git config --global user.name 'YOUR USERNAME'`
<br/>
`git config --global user.email 'YOUR EMAIL'`
<br/>

Hopefully it does not have to be said to substitute in your own GitHub username and email here. You can access this at any point just by finding the 'Shell' within Windows. Or, if you right click on any folder on your Desktop that is linked to a GitHub repo, you can open up the Shell instantly and Bash away.

What this stage has done is configure Git, which is software that runs on your desktop, to GitHub, which is a repository website.

Restart R Studio. Whew, that was tough. Next.

<br/>

## Step three: Why did I just do that? <a name="three"></a>

OK, hold your breathe, we're going to pause here just to learn some basic Git commands. Some of the key ones you could do with learning are:

* **Add**: This is where you submit files to the staging area before being committed.

* **Commit** This is like 'saving' your work by creating a new version or copy.

* **Push**: This is how you send files from your local project to the online repository.

* **Pull**: This is how you get files from your online repository to your local project.

Back in RStudio, type in the following into the *Terminal*, or by opening up a new Shell:

`git add .`

It won't actually do anything for now, but in the future will add all files in your current working directory (that's what the `.` does) to staging ready for a commit.

<br/>

## Step four: The perfect marriage between Git and R <a name="four"></a>

Now, in Task 1, you should have learned how to build your very first GitHub repository. If you haven't done that, we can wait here while you go and do that. If you have already, or have an existing GitHub repository, we can move on.

So, you should have a repository on GitHub, complete with a `README` file, a `LICENSE` file and some other bits and bobs.

What we are going to do now, is integrate that repository with Git. Steady now.

1. Firstly, go to **Project > Create Project > Version Control > Git**.
2. Back on GitHub, you should see a bit where there is a https:// URL. That is the link to your repository, and it gives you the option to clone it in your desktop. For now, just copy that link, switch back to RStudio, and paste it into the 'Repository URL' as indicated.
3. Give the project a directory name, like test, Jim, or whatever you want.
4. Next, browse for the place on your desktop where you want this project to live, its subdirectory.
5. Click 'Create Project', and let the magic be done!

What you just did was tell RStudio to associate a new project in R with specific repository on GitHub.

## **Step four: Alternative**

If you still haven't built your first repository on GitHub, we can do something slightly different here. In RStudio, click *New project* and then *New Directory*. Call it what you want and change the directory as needed, make sure to tick *Create a git repository*, and then click *Create Project*. This creates an `.Rproj` file, which you can manage in the usual way through RStudio, including adding `README.md`and `LICENSE.md` files as discussing in Task 1.

## Step five: Getting content with content <a name="five"></a>

Remember that `README` file we created a while back? Well, it's time to write it. Thinking back to Task 1, there were some specific things that we said make a good `README` file. Do you remember what any of them were? Just to refresh your memory, these were:

* What is this project about and what does it do.
* Why should people care, and why is it useful.
* How can someone get started contributing to the project.
* Who can be contacted in case someone needs help.
* A link to the license, contributing guidelines, and code of conduct.
* A description of the project structure.
* Who is involved, and what are their roles.
* The current status of the project.

So, in RStudio, open that file try adding just a bit of information about this for your project. If you are doing this for an actual project, try and make it useful. If you are just tinkering for now, you can add what you want.

Remember that your `README` file is in markdown (.md) format. For a refresher on some of the simple syntax markdown uses, check this [handy cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).

<p align="center">
  <img src="https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/images/markdown.png?raw=true" width="600px"/>
</p>

<p align="center"><i>Screenshot of what this module looks in markdown, during development. Meta.</i></p>

<br/>

## Step six: A brave commitment <a name="six"></a>

OK, so now you should have a nicely edited `README` file. Now we are going to 'commit' this to the project using Git. This is basically the equivalent of saving this version of your project, with a record of what changes were made. Successive commits produce a history that can be examined at a later time, allowing you to work with confidence.

There are a few ways of doing this.

1. Go to **Tools > Version Control > Commit**
2. In the environment pane in RStudio, there should be a new 'Git' tab. Handy.
3. In your console pane, there should now be a new 'Terminal', which you can run Git command lines through.

Let's just stick with the second option for now. This Git pane shows you which files have been changed and includes buttons for the most important Git commands we saw earlier.

Select the `README` file in the Git window, which should show up automatically if you have made any edits to it. This adds that file to the 'staging' area, which is sort of like the pre-saving space for your work. Click 'Commit' and a new window should pop up.

Here, you have a chance to review your changes, and write a nice commit message. Type in something brief, but informative about the changes that you have made in this version or snapshot of your work. You want this to be enough information so that if you or someone else looks back on it, you'll know why you made this commit and the changes associated with it. These are like safety nets for your project in case you need to fall back for some reason.

> **Pro-tip**: Here, you will see a list of all the changes you have made since your last commit. Older removed lines are in red, and newly added lines are in green. Double check these to make sure that the edits you have made are the ones you intended to make. This is really helpful for spotting typos, stray edits, and any other little mistakes you might have accidentially introduced. Safety first.

**Note** If you are colour-blind and can't see which lines have been added or removed, you can use the line numbers in the two columns on the left of the window as a guide. Here, the number in the first column identifies the older version, and the number in the second column identifies the new version.

Now when you click 'Commit', another window will pop up, telling you how many files you have changed and the number of lines within that file you have changed. Close that little window down.

<br/>

## Step seven: PUSH! <a name="seven"></a>

Click the *Push* button in the top right of the new window. A new window will pop up now. What this is doing is synchronising the files changed on your local repository with the `README` file to the online version of the project on GitHub.

To do this from the Shell, use the following command:

`git push -u origin master`


Some times here you will be prompted to add your username and password from GitHub, which you should do if asked.

Close that window down, and the next one. Go to your project on GitHub, refresh, and check that the `README` file is still there in all its newly edited glory. You should see the commit message you made next to the file too.

<br/>

**OPTIONAL ADVANCED/AWESOME STEP**

Alright, so you just pushed some content to your first repo, awesome! Now let's put it into practice for a real project. Like, the one you are participating in right now. Let's try this out:

1. Go to the repositors for this project on [GitHub](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source)

2. Fork the repository to your own GitHub account. The URL for this should be: `https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source.git`

3. Head into RStudio, go to **File > New Project**, choose *Version Control*, select *Git*, and then paste the forked repository URL found in your copy of the repository. You now have your own versioned copy of this whole module. Neat. Save this somewhere on your local machine.

4. Now, you need to tell Git that a different version of this project exists. Open up the *Shell*, and enter the command: `git remote add upstream https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source`

5. What you just did was name the original branch here `upstream`, just to keep things simple for now. Now, create a new **branch** to document your changes to this independent of the main branch. Enter the command: `git checkout -b proposed-changes master`

6. You just created a new branch called `proposed-changes` where you can now edit all of the content and files to your heart's delight. Hopefully, the structure of this project is simple enough for you to navigate around. All of the raw files for the MOOC can be found in the `content_development` folder, and this is `Task_3.md`.

7. If you scroll to the bottom of `Task_3.md`, you should see a place where you can edit in your name and affiliation. Add these in, and then go through the commit procedure detailed above. If you see anything else that needs editing too, feel free to add them in too!

8. Now, you want to push the changes back to the original branch. Use the following command in your *Shell*: `git push origin proposed-changes`

9. Go back to GitHub and find your fork here. Click the little green button, and create a pull request. This is essentially a review to integrate the changes made into the original branch for this MOOC project.

10. The owners in charge of the MOOC project will now get a notification of this, review it, and confirm it if everything went to plan! We will review it, and if it all went okay, your name will now appear for all eternity as someone who completed this advanced task.

11. Have a cup of tea, coffee, or wine to celebrate!

**CONGRATULATIONS**

You just integrated Git with R Studio, and made your first change to a version controlled project. Your life will now never be the same, and your research workflow will probably be more rapid, agile, and collaborative than ever. Good luck going back to Word.

The great thing is that this doesn't have to just be used for code. You can use it for plain text, markdown, html, and, well, R code. The possibilities are limitless - what you have just learned is a new form of openly collaborative project management that works for an enormous range of tasks.

From now on, it is all up to you! Some advice is to:

* Make frequent commits. Treat Git like your puppy, in that it requires constant and special attention. Just a pat on the head every now and then is enough to keep it satisfied, but it'll be happiest with sustained servicing.

* The best way to do this is to make a commit each time you work on a specific problem. For example, writing a paragraph, running an analysis, or fixing a bug.

* Push often. Don't let those commits build up, otherwise you run more risk of getting into merge conflicts. Seeing as these can be the stuff of nightmares, just make sure to push often.

* Pull often. If others are working remotely on the same project, you will want to stay up to date with their changes. Make sure to frequently pull in their changes from GitHub to make sure you are all in sync.

* Experiment and explore! This task really only scratches the surface, and there are many different functions, tools, and ways this can be used. Really, it is up to you to find out how to use this information to improve your research workflow, and ultimately collaborate on better, more open and reliable research!

* To learn more about issues, branches, merge conflicts, pull requests, and other advanced aspects of using Git and RStudio, check out this [awesome guide](http://r-pkgs.had.co.nz/git.html) by Hadley Wickham.

<br/>

**Know a way this content can be improved?**

Time to take your new GitHub skills for a test-run! All content development primarily happens [here](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/Task_3.md). If you have a suggested improvement to the content, layout, or anything else, you can make it and then it will automatically become part of the MOOC content after verification from a moderator!

## List of participants who completed the ADVANCED version of this task

* Brendan Palmer,CRF-C, University College Cork
* Lisa Matthias, Freie Universität Berlin
* Hollie Marshall, University of Leicester 
* Eric D. Wilkey, Western University, Canada
* José-Raúl Canay-Pazos, Universidade de Santiago de Compostela, Spain
* Encarnación Martínez Álvarez, Spain


[![CC0 Public Domain Dedication](https://img.shields.io/badge/License-CC0%201.0-lightgrey.svg)](https://creativecommons.org/publicdomain/zero/1.0/)
