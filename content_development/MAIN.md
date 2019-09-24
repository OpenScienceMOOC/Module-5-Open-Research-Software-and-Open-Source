---
output:
  html_document: default
  pdf_document: default
---

# Module 5: Open Research Software and Open Source

## Table of Contents

 - [Introduction](#Introduction)
 - [What is Open Source Software](#What_OSS)
 - [Principles of Open Source Software](#Principles)
 - [The Open Source community and its governance](#OS_Community)
 - [Existing platforms and tools for Open Source Software](#Platforms)
 - [Open Source Software used in research](#Research)
 - [Getting Started with OSS - FAQ](#FAQ)
 - [Making good software for re-use](#Reuse)
 - [Open Source licensing](#Licensing)
 - [Software citation](#Citation)
 - [Using GitHub and Zenodo](#GitHub_Zenodo)
 - [Collaborating through Open Source](#Collaborating)
 - [Where to go from here](#Future_OSS)

**PLEASE NOTE** that an audio version of this is available to download via [Soundcloud](https://soundcloud.com/open-science-mooc/module-5-open-source-and-open-research-software) and [YouTube](https://www.youtube.com/watch?v=BHrOEmKk5zM).

## Introduction <a name="Introduction"></a>

Welcome to **Module 5** of the Open Science MOOC: **Open Research Software and Open Source**.

This module has been developed [in the open](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source) through collaboration by an international team of [Open Source afficianados](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/README.md#development-team-). Everything you see here has been developed in the open through interactive feedback and collaboration from the wider community. It comprises a series of videos, infographics, text-based reading, and practical tasks for you to sink you teeth into.

Don't forget you can join in the discussions over at our open [**Slack channel**](https://osmooc.herokuapp.com/). Please do introduce yourself at #module5opensource, and tell us a bit about who you are, your background, and how you ended up here!

### Who is this module for?

This module is designed primarily for computational researchers at the graduate and undergraduate level, as well as budding data scientists and any other researcher who uses analytical code or software. In a modern day research environment, this covers pretty much anyone who uses a computer for ther work.

> "An article about computational result is advertising, not scholarship. The actual scholarship is the full software environment, code and data, that produced the result." - J. Buckheit and D. L. Donoho, 1995.

Software and technology underpin much of modern research, which is now almost inevitably computational in one way or another - search engines, social networking platforms, analytical software, and digital publishing. With this, there is an ever-increasing demand for more sophisticated Open Source Software, matched by an increasing willingness for researchers to openly collaborate on new tools.

The power of Open Source is in that it lowers the barriers to collaboration and adoption, therefore allowing ideas and technology to spread more rapidly. This Module will introduce the necessary tools required for transforming software into something that can be openly accessed and re-used by others.

<img src="https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/images/open_research_software_open_source.png?raw=true" width="800" />

<p align="center"><i>Image by Patrick Hochstenbach (CC0 1.0 Universal)</i></p>

<br/>

### **Specific learning objectives for this Module**:

1. Learn the characteristics of open software; understand the **ethical, legal, economic, and research impact arguments for and against Open Source Software**, and further understand the quality requirements of open code.

2. Be able to turn code made for personal use into open code which is accessible by others.

3. Use software (tools) that utilizes open content and encourages wider collaboration.

<br/>

## What is Open Source Software <a name="What_OSS"></a>

Virtually all modern scientific research workflows rely on a range of software tools, either operating on different datasets, with different parameters, and applied iteratively in various ways (data science) or operating on different inputs and using models and methods to predict some output state (computational science). Open Source Software (OSS) is computer software in which the full source code is available under a specific license that enables other users to access, view, modify, and redistribute that code for any purpose. Because OSS requires such a license, it typically remains free of charge by default. This explicit licensing is also what differentiates OSS from free software. Re-using OSS for analysis, simulation and visualisation for research is also typically easier and more flexible compared to proprietary software. Often, whether we know it or not, we are already using OSS as part of our own research workflows.

OSS fits into the broader scheme of Open Science as it helps to make the full research environment, including the software that produced the research results, fully accessible and re-usable. As such, it forms a necessary component for the best practices ([Jiménez et al., 2018](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/Reading%20Material_Open%20Source%20and%20Open%20Research%20Software/Jim%C3%A9nez%20et%20al.%2C%202018.pdf)) and repeatability and reproducibility of research (both personally and by others), along with other components, such as sharing data ([Stodden, 2010](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/Reading%20Material_Open%20Source%20and%20Open%20Research%20Software/Stodden%2C%202010.pdf)).

In some cases, sharing of source code can even be conditional for the acceptance of associated research manuscripts ([Shamir et al., 2013](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/Reading%20Material_Open%20Source%20and%20Open%20Research%20Software/Shamir%20et%20al.%2C%202013.pdf)). It is also generally perceived to increase research impact ([Vandwalle, 2012](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/Reading%20Material_Open%20Source%20and%20Open%20Research%20Software/Vandewalle%2C%202012.pdf)).

Some of common advantages for developers include:

- Increased developer loyalty and empowerment;

- Lower costs of services and marketing;

- Increased branding of services and products;

- Production of high quality software at lower expense;

- Flexibility and rapid innovation;

- Customisation and modular integration;

- Increased reliability and independence; and

- Based on open standards available to everyone.

As such, the main advantages for researchers (users) include **lower costs**, **increased transparency**, **increased security and stability**, **no vendor 'lock in' with increased user control**, and **overall higher quality**. Furthermore, sharing OSS allows researchers to receive credit for their efforts, for example through direct software citation [(Smith et al., 2016)](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/Reading%20Material_Open%20Source%20and%20Open%20Research%20Software/Smith%20et%20al.%2C%202016.pdf).

Commonly used OSS include the [Mozilla Firefox](https://www.mozilla.org/en-US/firefox/) internet browser and the [LibreOffice](https://www.libreoffice.org/) full office suite. LibreOffice is similar to the popular Microsoft Office, including a word processor, spreadsheet manager, and slide presentation software, but is completely free and Open Source.

Some regard the OSS movement to represent a counter-movement to neoliberalism and privatisation, through defiance of regulations and norms in the construction and re-use of information, and a potential transformation of modern-day capitalism through making software abundantly available with minimal effort. See [The free/open source software movement: Resistance or change?](https://doi.org/10.15448/1984-7289.2009.1.5569) by Panayiota Georgopoulou for more on this topic.

<br/>

## Principles of Open Source Software <a name="Principles"></a>

The [Open Source Initiative](https://opensource.org/), one of the pioneers of OSS, offers the following [definition](https://en.wikipedia.org/wiki/The_Open_Source_Definition#Definition):

*Don't worry, you don't need to memorise all of this, but it's good to know the principles that OSS is coming from.*

 - **Free Redistribution**: The license shall not restrict any party from selling or giving away the software as a component of an aggregate software distribution containing programs from several different sources. The license shall not require a royalty or other fee for such sale.

- **Source Code**: The program must include source code, and must allow distribution in source code as well as compiled form. Where some form of a product is not distributed with source code, there must be a well-publicized means of obtaining the source code for no more than a reasonable reproduction cost preferably, downloading via the Internet without charge. The source code must be the preferred form in which a programmer would modify the program. Deliberately obfuscated source code is not allowed. Intermediate forms such as the output of a preprocessor or translator are not allowed.

- **Derived Works**: The license must allow modifications and derived works, and must allow them to be distributed under the same terms as the license of the original software.

- **Integrity of The Author's Source Code**: The license may restrict source-code from being distributed in modified form only if the license allows the distribution of "patch files" with the source code for the purpose of modifying the program at build time. The license must explicitly permit distribution of software built from modified source code. The license may require derived works to carry a different name or version number from the original software.

- **No Discrimination Against Persons or Groups**: The license must not discriminate against any person or group of persons.

- **No Discrimination Against Fields of Endeavour**: The license must not restrict anyone from making use of the program in a specific field of endeavour. For example, it may not restrict the program from being used in a business, or from being used for genetic research.

- **Distribution of License**: The rights attached to the program must apply to all to whom the program is redistributed without the need for execution of an additional license by those parties.

- **License Must Not Be Specific to a Product**: The rights attached to the program must not depend on the program's being part of a particular software distribution. If the program is extracted from that distribution and used or distributed within the terms of the program's license, all parties to whom the program is redistributed should have the same rights as those that are granted in conjunction with the original software distribution.

- **License Must Not Restrict Other Software**: The license must not place restrictions on other software that is distributed along with the licensed software. For example, the license must not insist that all other programs distributed on the same medium must be open-source software.

- **License Must Be Technology-Neutral**: No provision of the license may be predicated on any individual technology or style of interface.

Now, this all might be a little complex to remember. However, it can be summarised as *making software as re-usable as possible for future works, while also being freely available*.

<br/>

## An Open Source checklist

There are a number of existing platforms and tools that support OSS and collaboration. The [Open Science Training Handbook](https://open-science-training-handbook.gitbook.io/book/) provides a check-list to use for evaluating the 'openness' of existing research software, based on the Open Source Definition above:

- [ ] Is the software available to download and install?

- [ ] Can the software easily be installed on different platforms?

- [ ] Does the software have conditions on the use?

- [ ] Is the source code available for inspection?

- [ ] Is the full history of the source code available for inspection through a publicly available version history?

- [ ] Are the dependencies of the software (hardware and software) described properly? Do these dependencies require only a reasonably minimal amount of effort to obtain and use?

Check, check, check, done! Simples.

<br/>

## The Open Source community and its governance <a name="OS_Community"></a>

There are two main camps within the free/libre and open source software (FLOSS) community: The **free software movement**, and the **open source software movement** (OSS). Both have differing ideologies based on user liberties and the practical applications of software. The term 'FLOSS' is used as a overaching neutral term to refer to both; libre being French and Spanish for 'free' in the context of freedom.

In a similar way that people active in the open science movement are heterogeneous in their assumptions and aims, different opinions exist in the FLOSS community as well. Recalling module 1, two of the schools of thought in open science were the _Pragmatic school_ and the _Democratic school_. While the former is driven by the assumption that research could be more efficient if scientists worked together, the latter wants to set straight an unequal distribution of knowledge. They probably both end up sharing their research, but each with different intentions.

This is roughly comparable to the OSS and the free software movement: The latter evolved around 1983 to protect what they call the four essential freedoms of a program's user. These include the freedom to run, copy, distribute, study, change and improve a program. Software that respects these freedoms with an appropriate license is considered 'free'. The four freedoms are seen as vital for a society as a whole in the sense that they only enable sharing, cooperation and ultimately freedom in general. In this sense the free software movement is a social movement that creates an ethical imperative.

The open source software movement, which splintered off in 1998, focuses on the practical advantages and does not campaign for principles. It is concerned with developing high-quality software, for which everyone's ability to obtain, modify and contribute back the source code is considered highly beneficial.

Among multiple conclusions they arrive at, access to a program's source code is a shared one. Software thus may be considered _free_, _open source_, or both, according to agreed-on definitions by the Free Software Foundation ([FSF](https://www.gnu.org/philosophy/free-sw.html)) and the Open Source Initiative ([OSI](https://opensource.org/osd)). The FSF argues that free software is a subset of OSS, with only a [fraction](https://www.gnu.org/philosophy/free-open-overlap.html) being open source but nonfree.

Thus, highlighting a particular license status of software in use—open source or free—is mostly about different philosophies, not about software not having the other status as well. Each movement has its share of problems explaining their term: _free_ means more than being gratis and _open source_ means more than having access to the source code. The [FSF](https://www.gnu.org/philosophy/open-source-misses-the-point.html) and the European counterpart [FSFE](https://fsfe.org/documents/whyfs.html) provide more information on this topic.

### For individual projects

A typical open source project has the following types of formal roles:

- **Author**: It is the  person that created the project
- **Owner**: The person/s who has administrative ownership over the organization or repository 
- **Maintainers**: Contributors who are responsible for driving the vision and managing the organizational aspects of the project. (They may also be authors or owners of the project.)
- **Contributors**: The user that has already contributed to the project.
- **Community Members**: People who use the project. They might be active in conversations, create new issues or express their opinion on the future project improvements.

Typically, roles are made public through either the `README` file, a Contributors file, or a separate team page for the project.

<br/>

## Existing platforms and tools for Open Source Software <a name="Platforms"></a>

Virtual environments and machines are becoming increasingly popular as high-powered research workflow enablers, and many of these are built upon OSS (e.g., operating systems, programming languages, and data processing frameworks). Popular services include [Google Cloud](https://cloud.google.com/compute/) and [Amazon Web Services](https://aws.amazon.com/), which also assist with database storage and content delivery, as well as computational power. [InsideDNA](https://insidedna.me/) is a computing platform for reproducible research in bioinformatics, genomics and the life sciences.

As mentioned [above](#What_OSS), LibreOffice provides an Open Source alternative to Microsoft Office. The two are almost completely compatible, just with different default file formats. For citation managers, [Zotero](https://www.zotero.org/) is the most popular Open Source alternative to proprietary platforms such as Mendeley or EndNote.

[Zotero](https://www.zotero.org/) uses the BibTeX (pronounced 'bib-tech') format, based on LaTeX (pronounced 'lay-tech'), and has browser plugins to make citation management simple. By integrating this with other software such as LibreOffice, it is now possible to have a fully Open Source research workflow in many cases.

### GitHub <a name="GitHub"></a>

> Did you know that this entire project was build as an open and collaborative community effort in [GitHub](https://github.com/OpenScienceMOOC/)?

[GitHub](https://github.com/) is a popular hosting site for both software and non-software content (often called 'notebooks'), with added capabilities for version control, project management and tracking, and storage services. GitHub is built on top of the OSS [Git](https://git-scm.com/), which enables users to work remotely to maintain, share, and collaborate on research software and other non-software based projects.

Version control is essentially a process that takes snapshots of the files in a repository, and tracks modifications to them. It records when the changes were made, what they were, and who did them. If several people are working on one file at once, any overlapping changes are detected, and must be resolved prior to continuing. This provides a much more streamlined and automated process than manually saving and recording changes as projects develop. It also avoids the inevitable lists of confusing named file versions...

<p align="center"><img src="https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/images/xkcd.png?raw=true" width="200" /></p>

<p align="center"><i>GitHub helps us to avoid, er, sub-optimal file naming conventions (source: XKCD)</i></p>

<br/>

One of the more popular and useful functions of GitHub is the [issue tracker](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/issues), which is used to organise OSS development. The above link takes you to the issue tracker for the development of this module! If you think there is something here that can improved, or you want to comment on, anyone can add or contribute to an issue there!

Other similar project hosting services include [BitBucket](https://bitbucket.org/), [GitLab](https://about.gitlab.com/), and [Launchpad](https://launchpad.net/). If the recent acquisition of GitHub by Microsoft is a bit off-putting to you, these are great alternatives.

However, we also know that GitHub can have quite a high learning curve. Which is why the first practical task for this MOOC will teach you how to set up your first GitHub project repository!

**[GO TO TASK 1: Building your first GitHub repository](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/Task_1.md)**

<br/>


## Open Source Software used in research <a name="Research"></a>

Especially in scientific research, Open Source Software usage and development has become practically the norm. There's a number of reasons for this beyond those that apply to the general acceptance of OSS by, for example, consumers, industry, or government. Among these reasons are:

- Increasingly, algorithms implemented in analysis software form an integral part of the methods described in scholarly publications. As such, it is completely at odds with rigorous peer review if these algorithm implementations are closed to outsiders.

- Scientific collaboration more often than not spans multiple institutions and distributed research networks where secrecy and command hierarchy is not maintained in a way that is 'necessary' for closed source development.

- Many computational analyses are run in virtualized environments (such as institutional, national, or international 'cloud' infrastructures) and hosted on multi-user servers. Closed-source, commercial software often disallows such usage.

- OSS development often relies on volunteers. In a time of budgetary constraints for scientific research, this is a clear advantage.

For these and other reasons, Open Source tools are very commonly used in scientific research. This includes usage in fields where many researchers are amateur developers themselves and rely on tools such as [R](https://www.r-project.org/) for statistical analysis and scripting, which, in the last decade, has almost completely displaced commercial software for statistical analysis such as SPSS or JMP in a lot of fields. In fields such as bioinformatics, that involve a lot of file handling of the outputs of DNA sequencing platforms, general purpose scripting languages such as [Python](https://www.python.org/) and commonly used libraries built on top of it (such as [biopython](http://biopython.org)) have become a vital part of the toolkit of many researchers.

<p align="center"><img src="https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/images/python.png?raw=true" width="400" /></p>

<p align="center"><i>Python</i></p>

<br/>

Tools such as R and Python are essentially software for writing software. Although programming is an increasingly common activity among researchers, of course not *every* scientist does this. One step away from programming is the chaining together of the inputs and outputs of various analysis tools in longer workflows. As an example from genomics, a very common workflow is to start out with high-throughput sequencing reads and then i) do basic quality control checks; ii) map the reads against a reference genome; iii) identify the points where the new data are at variance with the reference. These steps are routinely executed as a workflow where a different Open Source executable is run in a Linux command-line environment for each of the three steps. Although this is arguably not quite open source software development, it does involve the usage and production of open source artifacts (such as Linux shell scripts) for which the principles that we discuss in this module are applicable.

<p align="center"><img src="https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/images/r.png?raw=true" width="200" /></p>

<p align="center"><i>R</i></p>

<br/>

Lastly, OSS is also used in scientific research for reasons that more closely mirror those that drive the adoption of OSS in wider society, namely that it is cheap. For example, individuals or organizations might decide to switch from Microsoft Office to LibreOffice for manuscript writing or spreadsheet processing because the latter is free (both as in [**'free beer'**](https://www.youtube.com/watch?v=dQw4w9WgXcQ) and 'free speech'). Likewise, the choice to switch from ArcGIS to [QGIS](https://www.qgis.org/en/site/) for the analysis of geographic information might be prompted simply by cost considerations.
<br/>

## Getting Started with OSS - FAQ <a name="FAQ"></a>

**I'm using X[e.g. Matlab,STATA,Excel] and I want to transition to something more open. What are the next steps?**

Even if you are using proprietary software, you can usually still share your source code/documents etc. *The best first step is sharing whatever you can*.  

**Great! I can put them in my new github repo.**

If that's enough for you for now great! If not for most pieces of proprietary software there are Open Source equivalents. Have a go with one and see what you think.  

| Closed | Open |
| --- | --- |
| Matlab | Python, Julia |
| STATA/SPSS | R |
| MS Office | LibreOffice |
| Mathematica | JupyterLab |
| Max/MSP | PureData |
| Test out your new [Pull Request -PR-](https://help.github.com/articles/about-pull-requests/) Skills ... | ... by adding your own example [here](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/MAIN.md) |

**Cool! But if I make the switch will I be stuck: taking ages to learn a new tool/ without support /with buggy software.**

Good question! The answer is it depends. The best thing to do is find someone who's made the switch before and learn from their experience. Or just do a Google search! Some OSS is much better than their closed counterparts, some aren't, so it's worth choosing carefully.  

## Making good software for re-use <a name="Reuse"></a>

The most likely person who might want to re-use your software in the future is...you! So while sharing is always better than not sharing, you can make your own life, and that of others, much easier through appropriate documentation. Documentation can include several things, such as including helpful comments and annotations in the code that help to explain why a particular action was performed, rather than what it is intended to achieve.

One of the most critical aspects of this is including an informative `README` file, that accompanies almost every OSS project, and some times even more than one. It can be a good practice to include one such file in every directory, that includes a list of files, a table of contents, and what the purpose of the directory is. The `README` file is typically just plain text or markdown (again, such as all of the ones for the MOOC!), and can include critical information for how to install and run software, previous dependencies and requirements, as well as tutorials or examples.

> **Did you know...** The term `README` is some times playfully ascribed to the famous scene in Lewis Carroll's Alice's Adventures In Wonderland in which Alice confronts magic munchies labeled with "Eat Me"" and "Drink Me". Potent.

The purpose here is to provide sufficient information to maximise the re-use and reproducibility of the computational environment, such that someone with no experience with the project can easily access and re-use the software ([Sandve et al., 2013](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/Reading%20Material_Open%20Source%20and%20Open%20Research%20Software/Sandve%20et%20al.%2C%202013.PDF)). By lowering the barriers to entry, you increase the chances of others being able to re-use your work, which is one of the ultimate goals of OSS ([Ince et al., 2012](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/Reading%20Material_Open%20Source%20and%20Open%20Research%20Software/Ince%20et%20al.%2C%202012.pdf)).

An extension of this that can help to make things even easier for future re-use is 'container' technology. Containers are like an ecosystem frozen in time, where the code, the data, any other dependencies, are all perfectly preserved, packaged and saved in the present functioning versions. This means that anyone in the future any one can come in and run the analyses again. As such, they are generally good for re-use, but this can come at the sacrifice of modification or understanding by others, as often a lot of details can be hidden within the source code and its dependencies. Common examples of container implementation in research include [Rocker](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/Reading%20Material_Open%20Source%20and%20Open%20Research%20Software/Boettiger%20and%20Eddelbuettel%2C%202017.pdf) (a Docker container for the R language), [Binder](https://mybinder.readthedocs.io/en/latest/), and [Code Ocean](https://codeocean.com/).

**Sustainable software is good software.**

<br/>

## 10 simple rules for reproducible computational research

The 10 simple rules for making computational research more reproducible, based on [Sandve et al., (2013)](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/Reading%20Material_Open%20Source%20and%20Open%20Research%20Software/Sandve%20et%20al.%2C%202013.PDF), are:

1. For every result, keep track of how it was produced.
2. Avoid manual data manipulation steps.
3. Archive the exact versions of all external programs used.
4. Version control all custom scripts.
5. Record all intermediate results, when possible in standardised formats.
6. For analyses that include randomness, note underlying random seeds.
7. Always store raw data behind plots.
8. Generate hierarchical analysis output, allowing layers of increasing detail to be inspected.
9. Connect textual statements to underlying results.
10. Provide public access to scripts, runs, and results.

<p align="center"><img src="https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/images/simple_rules.png?raw=true" width="800" /></p>

<p align="center"><i>Infographic adapted from Sandve et al., (2013). Feel free to download this and print it out to keep handy during your research!</i></p>

<br/>

If you follow these steps, along with the processes in [**Task 1**](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/Task_1.md) and [**Task 2**](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/Task_2.md), you should be fine!

<br/>

## Open Source licensing <a name="Licensing"></a>

An Open Source license is a type of license designed specifically for software and code that make it explicit what the legal conditions for sharing and re-use are. As mentioned [above](#What_OSS), the addition of a suitable license is what differentiates publicly shared software from OSS. For example, the widely used [MATLAB](https://www.mathworks.com/products/matlab.html) is proprietary software, and [Octave](https://www.gnu.org/software/octave/) is an openly licensed alternative programming language.

There are currently more than 1,400 unique Open Source licenses, a complexity born from the difficulty in understanding the differences between the legal implications across different license.

Some of the more common licenses include:

- [Berkeley Software Distribution ("BSD")](https://en.wikipedia.org/wiki/BSD_licenses),
- [Apache](https://www.apache.org/licenses/LICENSE-2.0),
- [MIT-style (Massachusetts Institute of Technology)](https://opensource.org/licenses/MIT), or
- [GNU General Public License ("GPL")](https://www.gnu.org/licenses/gpl-3.0.en.html).

You don't need to know all the legal itty gritty behind all of these, but it is good to at least know what options are avaiilable to you.

There are two ways in which contributions to a project become licensed:

1. *Explicitly*, whereby the individual contribution has a clearly indicated license independent of the main project; or
2. *Implicitly*, whereby the contribution falls under the original licensing code of the main project.

Thankfully, the process of selecting an Open Source license is relatively trivial, thanks to user-friendly tools such as [Choose A License](https://choosealicense.com/) or [Public License Selector](https://ufal.github.io/public-license-selector/). Each of these licenses allows other users to use, copy, distribute, and build upon your work, often while ensuring that the creators are appropriately recognised for their work. Here, the key is selecting an appropriate license for your work, depending on what you want, or do not want, others to do with it.

<br/>

## Software citation <a name="Citation"></a>

Citations provide one of the most important interactions in scholarly research, forming the basis of our referencing and metrics systems. Typically, this is performed thanks to the assistance of a permanent unique identifier such as a [Digital Object Identifiers](https://en.wikipedia.org/wiki/Digital_object_identifier) (DOI). A DOI is a persistent identifier, implemented in the [Handle System](https://en.wikipedia.org/wiki/Handle_System), that meets a common standard, depending on the purpose, such as for identifying academic information. Such identification is critical for tracking the genealogy and provenance of research, for reproducibility, as well as for giving appropriate credit to those who have created the software. Importantly, software should be considered a legitimate output from scholarly research, and citation is becoming an increasingly common way to indicate that.

In 2016, [Smith et al., 2016](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/Reading%20Material_Open%20Source%20and%20Open%20Research%20Software/Smith%20et%20al.%2C%202016.pdf) wrote a research paper about the principles of software citation as part of the FORCE11 Software Citation Working Group. In the same way that you would want to cite software that you have used as part of good research practices, it is important to make your research easily citable too. When citing any software used for your own research, you should include at minimum:

- The author name(s),
- Software title,
- Version number, and
- The unique identifier/locator (DOI or URL).

The six principles of software citation by [Smith et al., (2016)](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/Reading%20Material_Open%20Source%20and%20Open%20Research%20Software/Smith%20et%20al.%2C%202016.pdf) are provided here:

* **Importance**: Software should be considered a legitimate and citable product of research. Software citations should be accorded the same importance in the scholarly record as citations of other research products, such as publications and data; they should be included in the metadata of the citing work, for example in the reference list of a journal article, and should not be omitted or separated. Software should be cited on the same basis as any other research product such as a paper or a book, that is, authors should cite the appropriate set of software products just as they cite the appropriate set of papers.

* **Credit and attribution**: Software citations should facilitate giving scholarly credit and normative, legal attribution to all contributors to the software, recognizing that a single style or mechanism of attribution may not be applicable to all software.

* **Unique identification**: A software citation should include a method for identification that is machine actionable, globally unique, interoperable, and recognized by at least a community of the corresponding domain experts, and preferably by general public researchers.

* **Persistence**: Unique identifiers and metadata describing the software and its disposition should persist - even beyond the lifespan of the software they describe.

* **Accessibility**: Software citations should facilitate access to the software itself and to its associated metadata, documentation, data, and other materials necessary for both humans and machines to make informed use of the referenced software.

* **Specificity**: Software citations should facilitate identification of, and access to, the specific version of software that was used. Software identification should be as specific as necessary, such as using version numbers, revision numbers, or variants such as platforms.

Note: For instructions on 'how to make your software citable' see the section [**Using GitHub and Zenodo**](#GitHub_Zenodo) below and [**Task 2: Linking GitHub and Zenodo**](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/Task_2.md).

<br/>

## Using GitHub and Zenodo <a name="GitHub_Zenodo"></a>

[GitHub](#GitHub) is a popular tool for project management, content storage, and version control. Note that GitHub itself is not OSS. However, Git, the tool which it is based on, is. Git is designed to help manage the source code files, and the updates to them, for a software-related project. However, it can also be extended to other non-software projects; for example, this [MOOC](https://github.com/OpenScienceMOOC/)!

However, getting research onto GitHub is just the first step. It is equally important to make it persistent and re-usable, which is why having a Digital Object Identifier (DOI) associated with it can be useful. The simplest way to do this is through a service called [Zenodo](https://zenodo.org/), which is a free and open source multi-disciplinary repository created by OpenAIRE and CERN, and can be used to assign a DOI to individual GitHub repositories. There is a [GitHub Guide](https://guides.github.com/activities/citable-code/) that explains the details, which involve linking GitHub repositories directly through to Zenodo so that when developers create formal releases for their software, Zenodo creates and archives a that version of the software.  

There's nothing special about using Zenodo for creating DOIs, other than its **free of cost**; other general repositories can also be used, such as [DataCite DOI Fabrica](https://doi.datacite.org/), or your own institutional repositories such as [Caltech's](https://www.library.caltech.edu/news/enhanced-software-preservation-now-available-caltechdata).

A lot of researchers might typically be afraid of sharing code which is incomplete, buggy, or imperfect. However, in the OSS community, such a practice of sharing 'raw' code is fairly commonplace. Sharing code openly enables others to re-use and improve it, as well as to engage in a deeper way with any research associated with it. This is one of the fundamental aspects of peer-collaboration, perhaps best exemplified by the traditional process of research manuscript peer review.

Task 2 will guide you through the process of linking a GitHub repository to Zenodo for archiving.

> **Did you know...** All content produced for this MOOC is available as part of a community in [Zenodo](https://zenodo.org/communities/open-science-mooc/)?

**[GO TO TASK 2: Linking GitHub and Zenodo](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/Task_2.md)**

<br/>

## Collaborating and contributing through Open Source <a name="Collaborating"></a>

Often, OSS is developed in a public, decentralised, collaborative manner between multiple contributors. The purpose of this is to enhance the diversity and scope of a project and its design, in order to become more beneficial and sustainable. Such an approach was famously likened to a 'bazaar' model by Eric Raymond, an early OSS proponent. One of the major guiding principles of this is that of **peer production**, which relies on self-organised communities to regulate the development of content, co-ordinated towards a shared goal or outcome.

OSS projects rely heavily on volunteer collaboration, which often entails a constant flux of newcomers in order to become productive and sustainable ([Steinmacher et al., 2014](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/Reading%20Material_Open%20Source%20and%20Open%20Research%20Software/Steinmacher%20et%20al.%2C%202014.pdf)). Creating the right social atmosphere for a project, and a welcoming engagement environment, are often critical to successful collaboraitons in OSS.

<br/>

## Where to go from here <a name="Future_OSS"></a>

Hopefully now you have come to see the importance of software as a cornerstone of modern science, and the importance that OSS plays in this.

The **learning outcomes** from this should be:

1. You will now be able to define the characteristics of OSS, and some of the ethical, legal, economic and research impact arguments for and against it.

2. Based on community standards, you will now be able to describe the quality requirements of sharing and re-using open code.

3. You will now be able to use a range of research tools that utilise OSS.

4. You will now be able to transform code designed for their personal use into code that is accessible and re-usable by others.

5. Software developers will be able to make their software citable, and software users will know how to cite the software they use.

<br/>

**BONUS TASK**

If you have completed [Task 1](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/Task_1.md) and [Task 2](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/Task_2.md), we also have a **BONUS TASK** for you, if you want to take your skills a step further. [Task 3](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/Task_3.md) will take you a step deeper into integrating Git into a typical research workflow by showing you how to integrate it with R Studio. It is recommended that you have completed the first 2 tasks before proceeding with this one.

However, your Open Source journey does not stop here! This was just the beginning, and there are some incredible resources out there if you would like to do or learn more:

* If you feel particularly inspired by this, you can endorse the [Science Code Manifesto](http://sciencecodemanifesto.org/), which is based on the five principles of code, copyright, citation, credit, and curation.

* To launch and develop your own project, the [Open Source Guides](https://opensource.guide/) program offers a range of practical guides and skills to help launch and advance your OSS projects.

* For a detailed look at OSS-based research workflows, the [Open Science, Open Data, Open Source](https://pfern.github.io/OSODOS/gitbook/) hand-guide by Pedro L. Fernandes and Rutger A. Vos is one of the top resources online.

* More formalised journal venues also exist for software-based articles, including [The Journal of Open Research Software](https://openresearchsoftware.metajnl.com/) and [The Journal of Open Source Software](https://joss.theoj.org/).  A list of such venues is also [available](https://www.software.ac.uk/which-journals-should-i-publish-my-software).

* The [PLOS Open Source Toolkit](https://channels.plos.org/open-source-toolkit) provides a global forum for Open Source hardware and software research and applications.

* The [NumFOCUS](http://www.numfocus.org) is a nonprofit organization that supports and promotes world-class, innovative, open source scientific software. Some of the projects they sponsor include:

  * [IPython](http://ipython.org) and [Jupyter Notebook](https://jupyter.org) initiatives.

  * [rOpenSci](http://ropensci.org), which promotes the open source R statistical environment for transparent and reproducible research.

  * To gain more hands on experience with OSS, the [Software Carpentry](https://software-carpentry.org/) community holds regular workshops to improve lab-based computing skills ([Wilson et al., 2017](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/Reading%20Material_Open%20Source%20and%20Open%20Research%20Software/Wilson%20et%20al.%2C%202017.pdf)).

<br/>

### Further reading <a name="Reading"></a>

*These references here are just the beginning. They include some of the most useful general overviews of the Open Source landscape in research. However, if you want to be find something more specific to your own research field, then that path is there for you to explore!*

* The Future of Research in Free/Open Source Software Development [(Scacchi, 2010)](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/Reading%20Material_Open%20Source%20and%20Open%20Research%20Software/Scacchi%2C%202010.pdf).

* The Scientific Method in Practice: Reproducibility in the Computational Sciences [(Stodden, 2010)](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/Reading%20Material_Open%20Source%20and%20Open%20Research%20Software/Stodden%2C%202010.pdf).

* The case for open computer programs [(Ince et al., 2012)](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/Reading%20Material_Open%20Source%20and%20Open%20Research%20Software/Ince%20et%20al.%2C%202012.pdf).

* Current issues and research trends on open-source software communities [(Martinez-Torres and Diaz-Fernandez, 2013)](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/Reading%20Material_Open%20Source%20and%20Open%20Research%20Software/Martinez-Torres%20and%20Diaz-Fernandez%2C%202013.pdf).

* Ten simple rules for reproducible computational research [(Sandve et al., 2013)](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/Reading%20Material_Open%20Source%20and%20Open%20Research%20Software/Sandve%20et%20al.%2C%202013.PDF).

* A systematic literature review on the barriers faced by newcomers to open source software projects [(Steinmacher et al., 2014)](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/Reading%20Material_Open%20Source%20and%20Open%20Research%20Software/Steinmacher%20et%20al.%2C%202014.pdf).

* Knowledge sharing in open source software communities: motivations and management [(Iskoujina and Roberts, 2015)](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/Reading%20Material_Open%20Source%20and%20Open%20Research%20Software/Iskoujina%20and%20Roberts%2C%202015.pdf).

* Software citation principles [(Smith et al., 2016)](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/Reading%20Material_Open%20Source%20and%20Open%20Research%20Software/Smith%20et%20al.%2C%202016.pdf).

* An introduction to Rocker: Docker containers for R [(Boettiger and Eddelbuettel, 2017)](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/Reading%20Material_Open%20Source%20and%20Open%20Research%20Software/Boettiger%20and%20Eddelbuettel%2C%202017.pdf).

* Good enough practices in scientific computing [(Wilson et al., 2017)](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/Reading%20Material_Open%20Source%20and%20Open%20Research%20Software/Wilson%20et%20al.%2C%202017.pdf).

* Four simple recommendations to encourage best practices in research software [(Jiménez et al., 2017)](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/Reading%20Material_Open%20Source%20and%20Open%20Research%20Software/Jim%C3%A9nez%20et%20al.%2C%202018.pdf).

<br/>

### Development Team <a name="Development_team"></a>

- [Alex Morley](https://twitter.com/alex__morley), Open Sourceror, University of Oxford, UK.
- [Kevin Moerman](https://twitter.com/KMMoerman), Open Sourceror, MIT, USA.
- [Tania Allard](https://twitter.com/ixek), Open Sourceress, Data Enchantress, University of Leeds, UK.
- [Simon Worthington](https://twitter.com/mrchristian99), Book Liberationist, TIB, Germany.
- [Paola Masuzzo](https://twitter.com/pcmasuzzo), Open Source Batman, Italy.
- [Ivo Grigorov](https://twitter.com/OAforClimate), Open Source Robin, Denmark.
- [Rutger Vos](https://twitter.com/rvosa), Open Sourceror, Naturalis Biodiversity Center, the Netherlands.
- [Julien Colomb](https://twitter.com/j_colomb), Open Ninja, Berlin.
- [Jon Tennant](https://twitter.com/protohedgehog), Dinosaur Whisperer.

**Know a way this content can be improved?**

Time to take your new GitHub skills for a test-run! All content development primarily happens [here](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/MAIN.md). If you have a suggested improvement to the content, layout, or anything else, you can make it and then it will automatically become part of the MOOC content after verification from a moderator!

[![CC0 Public Domain Dedication](https://img.shields.io/badge/License-CC0%201.0-lightgrey.svg)](https://creativecommons.org/publicdomain/zero/1.0/)
