# Contribution Guidelines

**New to GIT and GitHub?** See [these learning resources](https://help.github.com/articles/git-and-github-learning-resources/) and this [10 min. GIT tutorial](https://try.github.io/levels/1/challenges/1).

These are the main contributing guidelines for the development of this MOOC, and apply to each module within. The development structure for this is based on a combination of two things:

* Invited experts as part of a core development team, led by one or two managers for each module.
* Open participation, where anyone can contribute using the standard processes on GitHub.

Feedback and contributions of any form are welcomed. Feel free also to [contact us](https://opensciencemooc.github.io/site/Contact/) to discuss anything further.

At the present, development is in early stages, as this is an entirely crowd-sourced and volunteer-led project. We are focusing inititally on [Module 5, Open Research Software and Open Source](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source) to run as a pilot for testing and receiving feedback. After this, the [protocol](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/tree/master/production_toolkit) and content will be revised, and then applied accordingly to the development of the remaining modules.

## Contact us

If you want to contribute, please firstly join our open [Slack channel](https://openmooc-ers-slackin.herokuapp.com/). Secondly, please add yourself to the [Development team](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source) on GitHub. Thirdly, please [add yourself](https://github.com/OpenScienceMOOC/site#how-to-add-a-person-to-be-listedrendered-on-the-website) to the main MOOC website.

If you have questions about the project, please [email us](info@opensciencemooc.eu) directly.

Stay tuned on what's happening on Twitter with [@OpenSci_MOOC](https://twitter.com/OpenScienceMOOC).

For partnerships, please see [here](https://opensciencemooc.github.io/site/About/).

## Getting started

* [Forming a team for collaborative design](https://github.com/OpenScienceMOOC/Main/blob/master/Production_Files/MODULE_DESIGN_PROTOCOL.md#forming-a-team-for-collaborative-design).

* [The development process](https://github.com/OpenScienceMOOC/Main/blob/master/Production_Files/MODULE_DESIGN_PROTOCOL.md#the-development-process).

* Familiarise yourself with the [script writing guide](https://github.com/OpenScienceMOOC/Main/blob/master/Production_Files/Writing_a_script.md), the [script template](https://github.com/OpenScienceMOOC/Main/blob/master/Production_Files/Script_template.md) and the [video management protocol](https://github.com/OpenScienceMOOC/Main/blob/master/Production_Files/Video_management_protocol.md).

Each team will adhere to the [MOOC planning template](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/production_toolkit/MOOC_planning_template.md) to structure development in a systematic way.

### Altering the module content.   

Modules are rendered from markdown files ([here is a useful markdown cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)) located in the [`content development`](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/tree/master/content_development) folder.

For each update made, make sure to update the [MOOC planning template](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/production_toolkit/MOOC_planning_template.md) as needed.


## Reporting issues

- **Search for existing issues.** Please check to see if someone else has reported the same [issue](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/issues).

- **Share as much information as possible.** Include operating system and version, browser and version. Also, include steps to reproduce the bug.

## Project Setup
Refer to the [README](README.md).

## Content style
This is flexible to each module as required, and defined by each development team in advance as part of the protocol.

## Code style
Flexible, as long as it is consistent. Ideally, all content would be drafted in markdown, for increasing re-use. This can be easily performed in R Studio, for example, which also has a GitHub interface to make collaborating on this project even simpler.

Please read [this guide](https://support.rstudio.com/hc/en-us/articles/200532077-Version-Control-with-Git-and-SVN) to familiarise yourself with this process. Which in itself, is actually fairly powerful for Open Science!

## Pull requests

Please refer to each project's style guidelines and guidelines for submitting patches and additions. In general, we follow the "fork-and-pull" Git workflow.

**NOTE: Be sure to merge the latest from "upstream" before making a pull request!**

- Fork the repo on GitHub
- Clone the project to your own machine
- Commit changes to your own branch
- Push your work back up to your fork
- Submit a Pull request so that we can review your changes


- Try not to pollute your pull request with unintended changes and keep them simple and small. If possible, squash your commits.
- Try to share how your code has been tested before submitting a pull request.
- If your PR resolves an issue, include **closes #ISSUE_NUMBER** in your commit message (or a [synonym](https://help.github.com/articles/closing-issues-via-commit-messages)).
- Review
    - If your PR is ready for review, another contributor will be assigned to review your PR.
    - The reviewer will accept or comment on the PR.
    - If needed address the comments left by the reviewer. Once you're ready to continue the review, ping the reviewer in a comment.
    - Once accepted your code will be merged to `master`.
