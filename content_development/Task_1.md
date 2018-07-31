# Task 1: How to set up a repository on GitHub

This task is designed for students and researchers who want to create their first Open Source project (software or non-software) on GitHub.

Estimated time to complete: 30-45 minutes.

## Table of contents

* [Getting started](#Getting_started)
  * [Setting up a GitHub profile](#Profile)
  * [The GitHub language](#Language)
  * [Creating a new repository](#Create_new)
* [The foundational steps](#Foundation)
  * [Choosing a license](#License)
  * [Creating a README file](#Readme)
  * [Creating contributing guidelines](#Contributing)
  * [Creating a code of conduct](#Conduct)
  * [Making your code citable](#Citation)
* [Keeping your issues up to date](#Issues)
* [Check-list for launching your project](#Check-list)

<img src="https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/images/Task1.png" alt="Task 1 workflow" width="2400" height="3444" style="margin-right: 30px; margin-left: 10px; float: left;" onmouseover="this.width='1200'; this.height='1722'" onmouseout="this.width='600'; this.height='861'">

<p align="center"><i>The workflow for Task 1. Keep this handy as you work through the task!</i></p>

## Getting started <a name="Getting_started"></a>

A 'repository' is really just a fancy name for a project on GitHub. GitHub is a place online where you can manage projects, store files, and openly collaborate with others. This is all achieved by using version control to track projects as they progress. As such, GitHub is a powerful tool for both software and non-software projects.

One of the most important things to consider at this early stage is to think about how you want the wider community to interact with your project. As you are working in the open, you want to make sure others feel comfortable in accessing, viewing, and engaging with your work. Setting up a repository in a way that lowers the barriers to entry, and the fear of being an 'outsider' is the first step towards maintaining a successful project.

<p align="center">
  <img src="https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/images/octocat.png" width="150px" height="125px"/>
</p>

<p align="center"><i>Octocat, GitHub's little mascot</i></p>

### Setting up a GitHub profile <a name="Profile"></a>

To set up a GitHub profile, simply head to the main page and click [Sign Up for GitHub](https://github.com/join). Here, you can create your personal account, with a username, email, and password as standard.

![Sign up for GitHub](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/images/github_signup.png)

<p align="center"><i>Sign up for GitHub</i></p>

The next step is to set up a personal plan. For now, simply select the 'Unlimited public repositories for free' plan, unless you are concerned about privacy, in which case select the private plan. If you intend to set up a project for an organisation, you can select that option too.


### The GitHub language <a name="Language"></a>

This is possibly the most confusing and off-putting aspect of GitHub. Here are some of the most commonly used terms and their definitions:

- **Initialise**: Create an empty repository.
- **Checkout**: Create a working copy of a local repository.
- **Clone**: Copy the repository into a local directory on your computer.
- **Fork**: Create a personal offshoot of a repository to work on it in parallel.
- **Branch**: An independent and parallel version of a repository. Changes do not affect the master branch.
- **Master**: The main and default branch for a repository.
- **Clean**: No commits pending on the branch.
- **Stage**: Add updates ready to be committed to a branch.
- **Commit**: A revision to a repository, like a versioned 'save' function.
- **Commit message**: A description of changes accompanying a commit.
- **Check**: A status check.
- **Fetch**: Nothing to do with dogs. Refers to getting the latest changes from an online repository without merging them.
- **Index**: The 'tree' which acts as a staging area.
- **Working Directory**: The 'tree' where the files are kept.
- **Head**: The 'tree' which indicates the last commits made.
- **Push**: Add committed changes to the head of your remote repository.
- **Merge**: Combining the changes made in one branch back with the master branch upon completion.
- **Pull**: Update your repository by fetching and merging the newest commits.
- **Pull request**: A request to merge an updated branch into the master branch.
- **Issue**: Suggested improvements, tasks, or questions related to a repository.

Whew! Don't worry about memorising *all* of these for now. Like any new skill, familiarity comes with experience.  

You can probably see how some of these are fairly similar to things like save, copy, paste - standard workflow operations, but adapted for a software management process. There are a [few more](https://mirrors.edge.kernel.org/pub/software/scm/git/docs/gitglossary.html) too, but this should do for getting started.

If you are interested, most of these terms come from the underlying [Git system](https://git-scm.com). Git was built to allow developers to manage different versions of source code in a distributed manner, which is great. It has lots of features and the ability to do lots of complex stuff, written by a [very clever guy](https://www.linuxfoundation.org/blog/10-years-of-git-an-interview-with-git-creator-linus-torvalds/).  However, the [user interface was not designed with new users in mind](https://xkcd.com/1597/), so it can be hard to learn. 


### Creating a new repository <a name="Create_new"></a>

On your GitHub profile, click the 'Create new repository'. The first step is to create a name as the brand for your project. Ideally, it should be memorable and give some indication of what the project does.

![Create a new repository](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/images/new_repo.png)

<p align="center"><i>Create a new repository</i></p>

Make sure not to duplicate names, infringe upon other trademarks, or name it anything that could be considered to be offensive.


## The foundational steps <a name="Foundation"></a>

Any GitHub repository requires 4 key elements to get started and to begin developing a welcoming community:

1. An Open Source license;
2. A README file;
3. Contributing guidelines; and
4. A Code of Conduct.

These are critical aspects and best practices of any project for users to understand their legal rights, their expectations, the purpose of the project, and to improve the overall user experience. 

All four of these files should be kept in the root directory for your project repository. It is convention to use markdown file formats (.md) for most of these files (though the license file is most often plain text (.txt)), and capitalise all file names. Instead of spaces in file names, make sure to use underscores _ . 

So you should end up with a foundational file selection like this:

1. LICENSE.md
2. README.md
3. CONTRIBUTING.md
4. CODE_OF_CONDUCT.md

![The basic repository structure](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/images/foundation.png)

<p align="center"><i>The basic repository structure</i></p>

### Choosing a license <a name="License"></a>

Choosing an appropriate license is what will differentiate your Open Source repository from publicly available software. While you are not obliged to choose a license, doing so guarantees that others will be able to modify, share, re-use, and build upon your project within a legal framework.

To start with, you want to check [Choose A License](https://choosealicense.com/) to find a license that best suits your intentions for the repository.

The three primary ones to choose from are:

* **MIT License**: A permissive license that lets people do whatever they want with your code as long as they provide appropriate attribution to you, and do not hold you liable.
* **Apache License 2.0**: Similar permissions to the MIT License, but also provides an express grant of patent rights from contributors to users.
* **GNU General Public License (GPL) v3**: A [copyleft](https://en.wikipedia.org/wiki/Copyleft) license that requires anyone who redistributes your code, or a derivative work, to make the source available under the same terms as the original license; also provides an express grant of patent rights from contributors to users.

Thankfully, when you start a new repository on GitHub, you are given the option to select an existing license from a drop-down menu.  You should always (with very few exceptions) use an existing license, since this is what potential users and contributors will see before they choose to use or contribute to your software.

![Choosing a license](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/images/license.png)

<p align="center"><i>Choosing an example license</i></p>

If they don't have one you want, you can add one you like manually. To do this, simply click 'Create new file' in the repository, and copy and paste an existing license text in. Name the file something like 'LICENSE.txt' or 'LICENSE.md' to make it clear, and keep it in the main repository folder (i.e., the root). Make sure to add a clean commit message, and you're done!


### Creating a README file <a name="Readme"></a>

When you initialise your new repository, there should be an option to do so with a README file. Just like Alice in Wonderland, these do exactly what they say - provide key information about the project. These are typically the first thing outside contributors will see when they come to your repository, so making them informative and welcoming is key.

![Part of the README file for this module](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/images/readme.png)

<p align="center"><i>Part of the README file for this module</i></p>

The file will originally be in markdown (.md) format. This is a lightweight markup language with a plain text format. To learn some basic markdown, see [this cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet). But for now, we can just use plain text.

There are several things you will want to include in your README file:

* What is this project about and what does it do.
* Why should people care, and why is it useful.
* How can someone get started contributing to the project.
* Who can be contacted in case someone needs help.
* A link to the license, contributing guidelines, and code of conduct.
* A description of the project structure.
* Who is involved, and what are their roles.
* The current status of the project.

Remember that not everyone coming to your project will be an expert, or understand what it is you are doing and why. Having a well-documented README file will enhance the user experience for people with a range of prior knowledge.

When the README file is included in the root directory, GitHub will automatically display this on the homepage of your repository. This means it is the first thing people will often see, so make it count!

> **Pro-tip**: Later on as your project develops, you might want to add FAQs based on community feedback, or a tutorial to help users understand how your project works.


### Creating contributing guidelines <a name="Contributing"></a>

Contributing guidelines are designed to communicate to potential contributors a short guide on how to engage with your project and community. You want to make sure to be welcoming, and indicate that you are eager for participants to engage with your project. Whenever a participant opens a new pull request or creates a new issue, they will see a link to your contribution file.

![Part of the CONTRIBUTING file for this module](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/images/contributing.png)

<p align="center"><i>Part of the CONTRIBUTING guidelines for this module</i></p>

Sticking with the all caps file names, the next step is to create a CONTRIBUTING file. Click 'Create new file', and make sure to save it in markdown format as before. This file will tell other users how they can engage with and participate in your project. This is the first step towards establishing a community around your project, so make it engaging, concise, and informative.

The CONTRIBUTING file should include information on:

* What sort of contributions you are looking for.
* How to suggest updates or new features.
* How to interact with the project using GitHub's functions (e.g., the pull request protocol).
* How to file a bug report or create an issue.
* The ultimate goal, vision, or roadmap for the project.
* How to contact those in charge of the project.
* Links to any external documentation or websites.

Here, you are essentially trying to encourage people to volunteer their time to advance your project. Make sure to be welcoming and friendly, and be precise about how people can engage. When writing this, make sure to think about it from the user perspective - how can you make their life easier when submitting pull requests and opening issues to make the whole project run more smoothly.

> **Pro-tip**: Consider starting off with a short thank you note for people taking the time to consider contributing - they have clicked on the file to learn more after all! If there are other methods of recognition that you have in mind, make sure to include them in here too.


### Creating a Code of Conduct <a name="Conduct"></a>

A code of conduct is important for setting the ground rules for expected behaviour and participation for project contributors, and is an easily referenced document for showing that your project team takes constructive dialogues seriously. Therefore, it is a critical element for creating and maintaining a healthy community that engages in a constructive and productive manner within a positive social atmosphere.

A code of conduct not only provides expectations of behaviour, but also describes who those expectations apply to, when they apply, what to do should a violation of the code occur, and what the action items for this will be. As such, points of contact need to be made clear in the code of conduct. Typically, this should be in a private way such as an email address. 

> **Pro-tip**: In case a violation needs to be reported about the person who receives those reports, make sure to include an option to contact a secondary party.

To add a code of conduct, you can create your own from scratch by adding a new markdown file, or use existing templates such as the [Contributor Covenant](https://contributor-covenant.org/). Name your file CODE_OF_CONDUCT.md, and make sure it is visible in the README file.

![Part of the CODE OF CONDUCT file for this module, based on the Contributor Covenant](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/images/code_of_conduct.png)

<p align="center"><i>Part of the CODE OF CONDUCT file for this module, based on the Contributor Covenant</i></p>

Making sure to enforce the code of conduct is important, as it shows that not only do you value the code, but you respect the influence that it has on your community. It is important to treat each member of the community with the respect, courtesy, and importance that they deserve. Should a violation occur, or a repeat offender makes consistent violations, it is best to refer to the [Open Source Guide](https://opensource.guide/code-of-conduct/#enforcing-your-code-of-conduct) to see how to enforce the code of conduct.


### Making your code citable <a name="Citation"></a>

If you want to make your code citable from the start, you should store the metadata needed for a citation from the start, by creating a [codemeta.json](https://codemeta.github.io) file or a [CITATION.cff](https://citation-file-format.github.io) file. Both will allow tooling that is currently being developed to automatically create citation information, rather than asking you to type it in a form later.

If you're interested, [cite.research-software.org](https://cite.research-software.org) provides further background information about software citation in academia.

## Keeping your issues up to date <a name="Issues"></a>

Issues are not necessarily problems with a project, but also suggestions for improvement, things to develop in the future, and comments and feedback about the project to work through. They can be openly shared and discussed with contributors as needed, sort of like a forum.

If you are a project lead, it is important to maintain a list of issues that make it clear to contributors what aspects of the project need attention. It is also important to engage with as many issues as possible from others in a positive manner, to show that you take their contributions seriously.

Key elements for issues include:

* An informative title and description;
* Coloud-coded labels/tags to help categorise and filter;
* Milestones to associate issues with specific features or project phases;
* Assignees indicate who is responsible for working on an issue;
* Comments for providing feedback.

![The issue tracker for the Open Scholarship Strategy project](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/images/issues.png) [source](https://open-scholarship-strategy.github.io/site/)

<p align="center"><i>The issue tracker for the Open Scholarship Strategy project</i></p>

Within issues it is possible to use @ mentions to notify other contirbutors about the issue, and to get the right people engaged in an effective manner. GitHub has an internal system of notifications, just like Facebook or Twitter, and can also send emails to people who are mentioned in the issue tracker. This can all be customised for individuals within the user settings.


## Checklist for launching your project <a name="Checklist"></a>

So now you are ready to launch your project, begin advertising it, and getting contributions! Before continuing, make sure that you have:

- [ ] Project has a memorable and informative name
- [ ] Project has a LICENSE file that is an exact copy of an Open Source license
- [ ] Complete documentation including a README, CONTRIBUTING, and CODE_OF_CONDUCT files
- [ ] Project has at least one clearly labelled issue
- [ ] Any code included at this stage is clearly structured and annotated


**Congratulations**, you have now launched an Open Source research project! Hopefully, from here on out, your work will act to benefit the wider community, forge new collaborations, and create new and fantastic opportunities for you all.

From now on, it is all up to you! Some advice is to:

* Write clean code;
* Have a well-structured project;
* Make frequent commits with clean messages;
* Keep projects well-documented;
* Have clear contributing guidelines;
* Make use of the description and tag functions;
* Don't fork someone else's repository unless you intend to work on them;
* Make sure to contribute to other people's projects too.
