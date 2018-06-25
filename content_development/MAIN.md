# Module 5: Open Research Software and Open Source

## Table of Contents

 - [Introduction](#Introduction)
 - [What is Open Source Software](#What_OSS)
 - [Principles of Open Source Software](#Principles)
 - [The Open Source community, governance, and contributions](#OS_Community)
 - [Existing platforms and tools for Open Source Software](#Platforms)
 - [Making good software for re-use](#Reuse)
 - [Open Source licensing](#Licensing)
 - [Software citation](#Citation)
 - [Using GitHub and Zenodo](#GitHub_Zenodo)
 - [Collaborating through Open Source](#Collaborating)
 - [Where to go from here](#Future_OSS)
 

## Introduction <a name="Introduction"></a>

Welcome to Module 5 of the Open Science MOOC: Open Research Software and Open Source. This module has been developed [in the open](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source) through collaboration by an international team of [Open Source afficianados](https://github.com/OpenScienceMOOC/Module-5-Open-Research-Software-and-Open-Source#development-team).

Software and technology underpin modern science, which is now almost inevitably computational to varying degrees. There is an ever-increasing demand for more sophisticated Open Source Software, matched by an increasing willingness for researchers to openly collaborate on new tools. The power of Open Source is in that it lowers the barriers to collaboration and adoption, therefore allowing ideas and technology to spread more rapidly. This Module will introduce the necessary tools required for transforming software into something that can be openly accessed and re-used by others.


### **Specific learning outcomes for this Module**:

* You will be able to define the characteristics of Open Source research software, and the ethical, legal, economic and research impact arguments for and against it.
* Based on community standards, you will be able to describe the quality requirements of sharing and re-using open code.
* You will be able to use a range of research tools that utilise open source software.
* You will be able to transform code designed for their personal use into code that is accessible and re-usable by others.
* Software developers will be able to make their software citable, and software users will know how to cite the software they use.


## What is Open Source Software <a name="What_OSS"></a>

Open Source Software (OSS) is computer software in which the source code is available under a specific license that enables other users to access, modify, and redistribute that code for any purpose. Typically, as a result of this, it is easier to obtain and re-use compared to proprietary software. Because OSS requires such a license, it typically remains free of charge by default.

Some of the common advantages include:

- Increased developer loyalty and empowerment;
- Lower costs of services and marketing;
- Increased branding of services and products;
- Production of high quality software at lower expense;
- Flexibility and rapid innovation;
- Customisation and modular integration;
- Increased reliability and independence; and
- Based on open standards available to everyone.

As such, the main advantages for researchers include lower costs, increased security and stability, no vendor 'lock in' with increased user control, and overall higher quality. Some commonly used services include the [Mozilla Firefox](https://www.mozilla.org/en-US/firefox/) internet browser and the [LibreOffice](https://www.libreoffice.org/) full office suite. LibreOffice is similar to the popular Microsoft Office, including a word processor, spreadsheet manager, and slide presentation software, but is completely free and Open Source.

Some regard the OSS movement to represent a counter-movement to neoliberalism and privatisation, through defiance of regulations and norms in the construction and re-use of information, and a potential transformation of modern-day capitalism through making software abundantly available with minimal effort.


## Principles of Open Source Software <a name="Principles"></a>

The [Open Source Initiative](https://opensource.org/), one of the pioneers of OSS, offers the following [definition](https://en.wikipedia.org/wiki/The_Open_Source_Definition#Definition):

 - *Free Redistribution*: The license shall not restrict any party from selling or giving away the software as a component of an aggregate software distribution containing programs from several different sources. The license shall not require a royalty or other fee for such sale.

- *Source Code*: The program must include source code, and must allow distribution in source code as well as compiled form. Where some form of a product is not distributed with source code, there must be a well-publicized means of obtaining the source code for no more than a reasonable reproduction cost preferably, downloading via the Internet without charge. The source code must be the preferred form in which a programmer would modify the program. Deliberately obfuscated source code is not allowed. Intermediate forms such as the output of a preprocessor or translator are not allowed.

- *Derived Works*: The license must allow modifications and derived works, and must allow them to be distributed under the same terms as the license of the original software.
Integrity of The Author's Source Code The license may restrict source-code from being distributed in modified form only if the license allows the distribution of "patch files" with the source code for the purpose of modifying the program at build time. The license must explicitly permit distribution of software built from modified source code. The license may require derived works to carry a different name or version number from the original software.

- *No Discrimination Against Persons or Groups*: The license must not discriminate against any person or group of persons.

- *No Discrimination Against Fields of Endeavor*: The license must not restrict anyone from making use of the program in a specific field of endeavor. For example, it may not restrict the program from being used in a business, or from being used for genetic research.

- *Distribution of License*: The rights attached to the program must apply to all to whom the program is redistributed without the need for execution of an additional license by those parties.

- *License Must Not Be Specific to a Product*: The rights attached to the program must not depend on the program's being part of a particular software distribution. If the program is extracted from that distribution and used or distributed within the terms of the program's license, all parties to whom the program is redistributed should have the same rights as those that are granted in conjunction with the original software distribution.

- *License Must Not Restrict Other Software*: The license must not place restrictions on other software that is distributed along with the licensed software. For example, the license must not insist that all other programs distributed on the same medium must be open-source software.

- *License Must Be Technology-Neutral*: No provision of the license may be predicated on any individual technology or style of interface.

Now, this all might be a little complex to remember. However, it can be summarised as making software as re-usable as possible for future works, while also being freely available. This principle of re-use is what separates OSS from 'Free Software'. Free and Open Source Spftware (FOSS) is an inclusive term to describe software that can be classified as both free and Open Source. A good example of FOSS is the [Ubuntu Linux](https://www.ubuntu.com/) operation system.

The big difference between free software and OSS is that the former must distribute updated versions under the same license as the original, whereas newer versions of OSS can be distributed under different licenses. FOSS combines the best of both worlds. 

These definitions have now become widely adopted, both by international governments, as well as some large organisations such as the [Mozilla Foundation] and the [Wikimedia Foundation].


## The Open Source community and its governance <a name="OS_Community"></a>

There are two main camps within the free software community: The free software movement, and the OSS movement. Both have differing ideologies based on user liberties and the practical applications of software. The term 'FLOSS' is used to reconcile these two political camps, and means 'Free/Libre and Open Source Software'; Libre being French and Spanish for 'free' in the context of freedom. 

Major organisations in the FLOSS space include the UK's [Software Sustainability Institute](https://www.software.ac.uk/),


## Existing platforms and tools for Open Source Software <a name="Platforms"></a>

[InsideDNA](https://insidedna.me/) is a computing platform for reproducible research in bioinformatics, genomics and the life sciences.

Virtual environments and machines are becoming increasingly popular as high-powered research workflow enablers. Popular services include [Google Cloud](https://cloud.google.com/compute/) and [Amazon Web Services](https://aws.amazon.com/), which also assist with database storage and content delivery, as well as computational power.

As mentioned [above](#What_OSS), LibreOffice provides an Open Source alternative to Microsoft Office. The two are almost completely compatible, just with different default file formats.

For citation managers, [Zotero](https://www.zotero.org/) is the most popular Open Source alternative to proprietary platforms such as Mendeley or Endnote.


## Making good software for re-use <a name="Reuse"></a>


## Open Source licensing <a name="Licensing"></a>

An Open Source license is a type of license designed specifically for software and code that make it explicit what the legal conditions for sharing and re-use are. There are currently more than 1,400 unique Open Source licenses, a complexity born from the difficulty in understanding the differences between the legal implications across different license.

Some of the more common licenses include:

- Berkeley Software Distribution ("BSD");
- Apache; 
- MIT-style (Massachusetts Institute of Technology); or 
- GNU General Public License ("GPL")


There are two ways in which contributions to a project become licensed.
1. Explicitly, whereby the individual contribution has a clearly indicated license independent of the main project; or 
2. Implicitly, whereby the contribution falls under the original licensing code of the main project.

Thankfully, the process of selecting an Open Source license is relatively trivial, thanks to user-friendly tools such as [Choose A License](https://choosealicense.com/). Zotero uses the BibTeX (pronounced 'bib-tech') format, based on LaTeX (pronounced 'lay-tech'), and has browser plugins to make citation management simple.



## Software citation <a name="Citation"></a>

Citations form one of the most important interactions in scholarly research, forming the basis of our referencing and metrics systems. Typically, this is performed thanks to the assistance of [Digital Object Identifiers](https://en.wikipedia.org/wiki/Digital_object_identifier) (DOI). A DOI is a persistent identifier or handle that meets a common standard, depending on the purpose, such as for identifying academic information.


## Using GitHub and Zenodo <a name="GitHub_Zenodo"></a>

** NOTE: THIS IS WHERE A PRACTICAL ACTIVITY WILL BE** [Task 1](Task_1.Rmd)

** NOTE: POSSIBLE TASK 2, SETTING UP A GITHUBE REPO**

Note that GitHub itself is not OSS. However, Git, the tool which it is based on, is. Git is designed to help manage the source code files, and the updates to them, for a software-related project. However, it can also be extended to other non-software projects; for example, this MOOC!

Other project hosting services include BitBucket, GitLab, and Launchpad.

One of the more popular and useful functions of GitHub is the issue tracker, which is used to organise OSS development. 

A lot of researchers might typically be afraid of sharing code which is incomplete, buggy, or imperfect. However, in the OSS community, such a practice of sharing 'raw' code is fairly commonplace. Sharing code openly enables others to re-use and improve it, as well as to engage in a deeper way with any research associated with it. This is one of the fundamental aspects of peer-collaboration, perhaps best exemplified by the traditional process of research manuscript peer review.


More formalised journal venues also exist for software-based articles, including [The Journal of Open Research Software](https://openresearchsoftware.metajnl.com/) and [The Journal of Open Source Software](https://joss.theoj.org/).



## Collaborating and contributing through Open Source <a name="Collaborating"></a>

Often, OSS is developed in a public, decentralised, collaborative manner between multiple contributors. The purpose of this is to enhance the diversity and scope of a project and its design, in order to become more beneficial and sustainable. Such an approach was famously likened to a 'bazaar' model by Eric Raymod, an early OSS proponent. One of the major guiding principles of this is that of peer production, which relises on self-organised communities to regulate the development of content, co-ordinated towards a shared goal or outcome.



## Where to go from here <a name="Future_OSS"></a>


Hopefully now you have come to see the importance of software as a cornerstone of modern science, and the importance that OSS plays in this. If you feel particularly inspired by this, you can endorse the [Science Code Manifesto](http://sciencecodemanifesto.org/), which is based on the five principles of code, copyright, citation, credit, and curation.

To gain more hands on experience with OSS, the [Software Carpentry](https://software-carpentry.org/) community hold regular workshops to improve lab-based computing skills.

To launch and develop your own project, the [Open Source Guides](https://opensource.guide/) program offers a range of practical guides and skills to help launch and advance your OSS projects.

### Further reading <a name="Reading"></a>

The Future of Research in Free/Open Source Software Development (Scacchi, 2010).
The Scientific Method in Practice: Reproducibility in the Computational Sciences (Stodden, 2010).
The case for open computer programs (Ince et al., 2012).
Code Sharing Is Associated with Research Impact in Image Processing (Vandewalle, 2012).
Current issues and research trends on open-source software communities (Martinez-Torres and Diaz-Fernandez, 2013).
Ten simple rules for reproducible computational research (Sandve et al., 2013).
Practices in source code sharing in astrophysics (Shamir et al., 2013).
A systematic literature review on the barriers faced by newcomers to open source software projects (Steinmacher et al., 2014).
Knowledge sharing in open source software communities: motivations and management (Iskoujina and Roberts, 2015).
An open source pharma roadmap (Balasegaram et al., 2017).
An introduction to Rocker: Docker containers for R (Boettiger and Eddelbuettel, 2017).
Upon the Shoulders of Giants: Open-Source Hardware and Software in Analytical Chemistry (Dryden et al., 2017).
Four simple recommendations to encourage best practices in research software (Jiménez et al., 2017).
Perspectives on Reproducibility and Sustainability of Open-Source Scientific Software from Seven Years of the Dedalus Project (Oishi et al., 2018).
Good enough practices in scientific computing (Wilson et al. ,2017).


### Development Team <a name="Development_team"></a>

- [Alex Morley](https://twitter.com/alex__morley), Open Sourceror, University of Oxford, UK.
- [Kevin Moerman](https://twitter.com/KMMoerman), Open Sourceror, MIT, USA.
- [Tania Allard](https://twitter.com/ixek), Open Sourceress, Data Enchantress, University of Leeds, UK.
- [Simon Worthington](https://twitter.com/mrchristian99), Book Liberationist, TIB, Germany.
- [Paola Masuzzo](https://twitter.com/pcmasuzzo), Open Source Batman, Italy.
- [Ivo Grigorov](https://twitter.com/OAforClimate), Open Source Robin, Denmark.
- [Jon Tennant](https://twitter.com/protohedgehog), Dinosaur Whisperer. 