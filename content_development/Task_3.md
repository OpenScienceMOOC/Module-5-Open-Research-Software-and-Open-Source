---
output:
  html_document: default
  pdf_document: default
---

# Task 3: How to integrate Git with R Studio

This task is designed for students and researchers who want to implement a system of version control within a standard R-based workflow. Your future research self will thank your for the convenience.

Don't forget you can join in the discussions over at our open [**Slack channel**](https://openmooc-ers-slackin.herokuapp.com/). Please do introduce yourself at #module5opensource, and tell us a bit about who you are, your background, and how you ended up here!

Estimated time to complete: 

Estimate time saving once complete: 

## Table of contents

* [Getting started](#Getting_started)
  * [Git](#Git)
  * [R Studio](#Rstudio)
* [Step one: Download all the things](#one)
* [Step two: Configure Git inside RStudio](#two)
* [Step three: Why did I just do that?](#three)
* [Step four: The perfect marriage between Git and R](#four)
* [Step five: Getting content with content](#five)

## Getting started <a name="Getting_started"></a>

Congratulations on making it this far! If you're reading this, you've survived pull requests, webhooks, and can probably even tell us know what the F in FOSS stands for (*not* Frustration, or any other F-word not often related to Open Source Software). Hopefully, you have overcome any skepticism or reluctance towards the benefits of GitHub and Open Source Software, and are ready to take the next step.

Before starting this Task, make sure you have already completed [Task 1](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/Task_1.md) and [Task 2](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/Task_2.md), so that you are more familiar with GitHub and some standard Open Source practices.

This task will teach you how to integrate the version control software, Git, with the popular coding environment, R Studio. And yes, it is Git as in gif or God, not Jit as in the wrong way of pronouncing things.

If you are one of those researchers who thinks that having code spread across multiple hard-drives that are waiting to break, Dropbox, Google Drive, or any other non-specialist software, this task is just for you. All of us are guilty of this sort of thing once in a while, but there are ways to do it that are better for you, future you, and those who might benefit from your work.

<p align="center">
  <img src="        " alt="Task 1 workflow" width="600" height="861" style="margin-right: 30px; margin-left: 10px;" onmouseover="this.width='1200'; this.height='1722'" onmouseout="this.width='600'; this.height='861'">
</p>

<p align="center"><i>The workflow for Task 3. Keep this handy as you work through the task!</i></p>

<br/>

### Geting Git <a name="Git"></a>

So, what is Git, and how is it different to GitHub? Git is a version control system, which enables you to save time-stamped copies of your work throughout the development process. It also works with non-code items too, like again, this MOOC, the majority of which was written in markdown in R Studio, and integrated with a Git/GitHub workflow.

This is important, as all research goes through changes, and some times we want to know what those things were. Did you delete some text that you now think is important? Version control will save that for you. Did your code used to work perfectly, but is now buggy beyond belief? Version control. It's a great way to avoid that chaotic state where you have multiple copies of the same file, but without a stupid and annoying file naming convention. `FINAL_Revised_2.2_supervisor_edits_ver1.7_scream.txt` will be a thing of the past.

GitHub is the platform that allows you to seamlessly share code from your workspace (e.g., laptop) to be hosted in an online space. So, sort of like the public interface to GitHub. The advantafes of this are:

1. You get to keep copies of all your work through time;
2. You can compare work through different copies through time, which helps to spot bugs or errors;
3. Other people can collaborate openly with your work; and
4. You have both a local and an online copy of your work that remain in sync.


### RStudio <a name="Rstudio"></a>

R studio is a popular coding environment for researchers who use the statistical programming language, R.


## Step one: Download all the things <a name="one"></a>

1. You should already have a GitHub account by now. If not, [sign up here](https://github.com/).
2. Download and install the latest version of R.
3. Download and install the latest version of [Rstudio](https://www.rstudio.com/products/rstudio/#Desktop). Oh, hey, looks it Open Source! Swish.
4. Download and install the latest version of Git.

For now, just choose all the usual default options for each install. Depending on which Operating System (e.g., Mac, Windows, Linux), this might be different for each of you. For now, and for the rest of this task, we're going to stick with doing things the easy-ish Windows way (but also provide some instructions for using the command line).

If you want, you can also download the [local version of GitHub](https://desktop.github.com/) and use it through the simple GUI  - Graphical User Interface. It's available on Windows and Mac and Linux, and can make your life a little easier, especially if you want to use a different platform to RStudio.

## Step two: Configure Git inside RStudio <a name="two"></a>

Right, that's the easy bit done. Next, go into RStudio, and in the tabs at the top go to Go to **Tools > Options > Git/SVN**. SVN is just another version control system like Git, and we don't need to worry about that here.

In the place where it says 'Git executable', add the pathway here to the git.exe file that you just downloaded. Make sure all the boxes here are ticked.

> **Pro-tip:** You see here where it says 'Use Git Bash as shell for Git projects?' This is the place where you can use the command-line to access Git from outside of RStudio. It's a powerful beast. 

Restart R Studio. Whew, that was tough. Next.

## Step three: Why did I just do that? <a name="three"></a>


OK, hold your breathe, we're going to learn some Git commands. Some of the key ones you could do with learning are:

* **Repository**: This is the location for all of the files associated with your project.

* **Add**:

* **Commit**

* **Push**:

* **Pull**:

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

So, in RStudio, try adding just a bit of information about this for your project. If you are doing this for an actual project, try and make it useful. If you are just tinkering for now, you can add what you want.

Remember that your `README` file is in markdown (.md) format. For a refresher on some of the simple syntax markdown uses, check this [handy cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).

<p align="center">
  <img src="https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/images/markdown.png" width="600px"/>
</p>

<p align="center"><i>Screenshot of what this module looks in markdown, during development. Meta.</i></p>

<br/>

## Checklist for integrating Git and R Studio <a name="Checklist"></a>


- [ ] 


**CONGRATULATIONS!** 



From now on, it is all up to you! Some advice is to:

* Make frequent commits. Treat Git like your puppy, in that it requires constant and special attention. Just a pat on the head every now and then is enough to keep it satisfied, but it'll be happiest with sustained servicing.

* Push often. Don't let those commits build up, otherwise you run more risk of getting into merge conflicts. Seeing as these can be the stuff of nightmares, just make sure to push often.


**Know a way this content can be improved?**

Time to take your new GitHub skills for a test-run! All content development primarily happens [here](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/Task_3.md). If you have a suggsted improvement to the content, layout, or anything else, you can make it and then it will automatically become part of the MOOC content after verification from a moderator! 
