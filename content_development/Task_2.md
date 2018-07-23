# Task 2: How to make your code citable using GitHub and Zenodo

This task is designed for researchers who want to create and re-use GitHub-based repositories in academic literature.

## Table of contents
- [Set up a GitHub repository](#Setup)
- [Choose your GitHub repository](#Choose)
- [Login to Zenodo](#Login)
- [Authorise GitHub to connect with Zenodo](#Authorise)
- [Select the repository to archive](#Archive)
- [Check repository settings](#Check)
- [Create a new release](#Release)
- [Getting a DOI](#DOI)
- [Checklist for citing your project](#Checklist)
- [Additional resources](#Resources)

## Set up a GitHub repository <a name="Setup"></a>

Pro-tip: Make sure to include a license and readme file in your repository. This will indicate to people the purpose of the project, and how they can engage with it in the future.

This preceding stage can been completed as part of [Task 1: Building a GitHub repository](Task_1.Rmd) for this module 'Module 5: Open Research Software and Open Source'.

## Choose your GitHub repository <a name="Choose"></a>

Once on your GitHub project setup, in the [github.com](https://github.com) website head to the 'Repositories' tab. Select which repository you would like to archive, and open it up.

## Login to Zenodo <a name="Login"></a>

Now head over to [zenodo.org](https://zenodo.org). [Zenodo](https://zenodo.org/) is a platform where you can permanently archive your code and other project elements. Zenodo does this by assigning projects a Digital Object Identifier (DOI), which also helps to make the work more citable. This is different to GitHub, which acts as a place where the actual work on a project takes place, rather than long-term archiving of it. At GitHub, content can be modfied, deleted, rewritten, and irreversably changed, which makes it a bit concerning to be used for longer lasting referencing purposes. Zenodo offers more security and permanence for research outputs.

If you already have a Zenodo account, this is easy. If not, follow the steps to create one — you can even login using your GitHub account to make things simpler, as Zenodo has a built in integration for it. This might be easier than creating yet another research account and profile.

## Authorise GitHub to connect with Zenodo <a name="Authorise"></a>

On the Zenodo website authorise it to connect to your GitHub account in the '[Using GitHub](https://zenodo.org/account/settings/github/)' section. Here, Zenodo will redirect you to GitHub to ask for permissions to use '[webhooks](https://developer.github.com/webhooks/)' on your repositories. You want to authorise Zenodo here with the permissions it needs to form those links.

If you are trying to give Zenodo access to an organisational repository, you (or an administrator) will need to make sure that Zenodo is granted third party access permissions. GitHub will send an authorisation email that needs confirming. At this point, back in the settings of your repository on GitHub, you also need to make sure that the repository is set to 'public', not private.

## Select the repository to archive <a name="Archive"></a>

If you have got this far, this means that Zenodo is now authorised to configure the repository webhooks that it needs to archive the repository and issue it a DOI. To do this, on the Zenodo website simply click the 'on' button next to your repository in the GitHub section.

## Check repository settings <a name="Check"></a>

Now you have set up a new webhook between Zenodo and your repository. In GitHub, click on the settings for your repository, and the Webhooks tab on the left hand side menu. This should display the new Zenodo webhook configured to Zenodo. Note, it may take a little time for the webhook listing to show up.

## Create a new release <a name="Release"></a>

The first time you archive a repository is known as the 'first release'. Each time you create a new version of that repository and archive it, you create a new release. This can be tracked in the 'releases' tab for your repository on GitHub (top center).

For the first archived version of your repository, click 'Create a new release'. Fill in the form and give some details as to what the release entails. For the first release, make sure to call it v1.0.0, as it standard practice.

Finally, click 'publish release', and your archive will be published and versioned.

To view your release on Zenodo you need to visit the '[Upload](https://zenodo.org/deposit)' tab.

## Getting a DOI <a name="DOI"></a>

This is sometimes referred to as DOI 'minting', and requires a couple of extra bits of information about the repository on Zenodo. On Zenodo click the '[Upload](https://zenodo.org/deposit)' tab in the main menu, and your newly uploaded repository should be there. Scroll down the page and fill in the extra information as needed, and then click 'Publish'.

Note: Only after this extra information has been added will your DOI become live. It may also take a short time for the DOI to become active.

The GitHub/Zenodo integration will now assign a DOI to each version/release of a project repository. This enables users to refer to and cite specific versions of projects. Also, the list of authors for the citation is automatically determined by the GitHub user account names used by the repository - this means no-one gets left out. Author details can be edited later on Zenodo. DOIs used in Zenodo are registered through the [DataCite](https://www.datacite.org/) service.

*Pro-tip*: Copy the URL for the DOI into the README file for your GitHub repo to make cross-linking even easier, as well as present a clear highlighted DOI badge for users to see and make use of your DOI. You only need to do this once with your first release DOI as it acts as a 'concept DOI' and is linked to all subsequent release DOIs.

**Congratulations!!**

Your GitHub repository is now archived in Zenodo, and with a DOI that can be versioned to reflect updates to the repository version through time. You should be able to see details of this on the GitHub Zenodo page for your repository. This also means that your archived projects can get picked up by other indexing services and search engines that use DOIs too.

Providing a long-term archive and a DOI for your work is required for others to be able to properly cite it, as this provides basic citation metadata. For Open Science, it is important to be able to cite the software that you use in your research, and this integrated workflow enables that to happen, in line with best practices for research citation. Furthermore, this practice is important in elevating the standard of software (and related projects) to that of the standard of other research outputs.

*Pro tip*: Is your research funded by an EU grant? Now you can directly connect your archived project to your grant by updating the grant section of the metadata on the project’s Zenodo record. This massively helps to increase its discoverability!

## Checklist for citing your project <a name="Checklist"></a>

So now you have a sustainably archived GitHub repository in Zenodo that is ready to be re-used and cited! Before continuing, make sure that you have:

- [ ] Linked your GitHub project to Zenodo. If you see a complete copy of your GitHub repo in Zenodo then things are working.
- [ ] Zenodo and GitHub integrated setup works nicely. For example have all the author names, and correct project title come across to Zenodo. If not, or if authors just have nicknames you can edit the names in Zenodo.
- [ ] Project has a first release, with a DOI. You should have a DOI displayed on your projects Zenodo page. This first DOI is called the 'concept DOI' and is the master DOI linking to all subsequent release DOIs. Copy this DOI link and embed it in your GitHub projects README page. Your done!

### Additional resources <a name="Resources"></a>

[Making your code citable](https://guides.github.com/activities/citable-code/) – GitHub Guides.
