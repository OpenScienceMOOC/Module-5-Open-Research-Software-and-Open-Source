---
title: "OSMOOC 5.1"
output:
  html_fragment
---

# Module 5: Open Research Software and Open Source

## Table of Contents

 - [Introduction](#Introduction)
 - [What is Open Source Software](#What_OSS)
 - [Principles of Open Source Software](#Principles)
 - [The Open Source community and its governance](#OS_Community)
 - [Existing platforms and tools for Open Source Software](#Platforms)


**PLEASE NOTE** that an audio version of this is available to download via [Soundcloud](https://soundcloud.com/open-science-mooc/module-5-open-source-and-open-research-software) and [YouTube](https://www.youtube.com/watch?v=BHrOEmKk5zM).

## Introduction <a name="Introduction"></a>

Welcome to **Module 5** of the Open Science MOOC: **Open Research Software and Open Source**.

This module has been developed [in the open](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source) through collaboration by an international team of [Open Source afficianados](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/README.md#development-team-). Everything you see here has been developed in the open through interactive feedback and collaboration from the wider community. It comprises a series of videos, infographics, text-based reading, and practical tasks for you to sink you teeth into.

Don't forget you can join in the discussions over at our open [**Slack channel**](https://osmooc.herokuapp.com/). Please do introduce yourself at #module5opensource, and tell us a bit about who you are, your background, and how you ended up here!

### Who is this module for?

This module is designed primarily for computational researchers at the graduate and undergraduate level, as well as budding data scientists and any other researcher who uses analytical code or software. In a modern day research environment, this covers pretty much anyone who uses a computer for ther work.

> "An article about computational result is advertising, not scholarship. The actual scholarship is the full software environment, code and data, that produced the result." 
>
> --- J. Buckheit and D. L. Donoho, 1995.

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

OSS fits into the broader scheme of Open Science as it helps to make the full research environment, including the software that produced the research results, fully accessible and re-usable. As such, it forms a necessary component for the best practices ([Jiménez et al., 2018](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/Reading_Material_OSS/Jim%C3%A9nez%20et%20al.%2C%202018.pdf)) and repeatability and reproducibility of research (both personally and by others), along with other components, such as sharing data ([Stodden, 2010](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/Reading_Material_OSS/Stodden%2C%202010.pdf)).

In some cases, sharing of source code can even be conditional for the acceptance of associated research manuscripts ([Shamir et al., 2013](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/Reading_Material_OSS/Shamir%20et%20al.%2C%202013.pdf)). It is also generally perceived to increase research impact ([Vandwalle, 2012](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/Reading_Material_OSS/Vandewalle%2C%202012.pdf)).

Some of common advantages for developers include:

- Increased developer loyalty and empowerment;

- Lower costs of services and marketing;

- Increased branding of services and products;

- Production of high quality software at lower expense;

- Flexibility and rapid innovation;

- Customisation and modular integration;

- Increased reliability and independence; and

- Based on open standards available to everyone.

As such, the main advantages for researchers (users) include **lower costs**, **increased transparency**, **increased security and stability**, **no vendor 'lock in' with increased user control**, and **overall higher quality**. Furthermore, sharing OSS allows researchers to receive credit for their efforts, for example through direct software citation ([Smith et al., 2016](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/Reading_Material_OSS/Smith%20et%20al.%2C%202016.pdf)).

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

Virtual environments and machines are becoming increasingly popular as high-powered research workflow enablers, and many of these are built upon OSS (e.g., operating systems, programming languages, and data processing frameworks). Popular services include [Google Cloud](https://cloud.google.com/compute/) and [Amazon Web Services](https://aws.amazon.com/), which also assist with database storage and content delivery, as well as computational power. InsideDNA (link dead.) is a computing platform for reproducible research in bioinformatics, genomics and the life sciences.

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

GO TO TASK 1!

[Task 1 also available on Github](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source/blob/master/content_development/Task_1.md)

<br/>