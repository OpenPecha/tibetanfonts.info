
# Writing the docs for a new repository

To ensure that OpenPecha products have user-friendly documentation, our new repo templates contain a documentation template. 

Completing the docs template is straightforward. You only need to:

1. [Update the docs site's config file](#1-update-the-docs-sites-config-file)
1. [Update the repository's README](#2-update-the-repositorys-readme)
1. [Fill out three (or more) content pages](#3-fill-out-three-or-more-content-pages)
1. [Publish the site by updating the repository's settings](#4-publish-the-site-by-updating-a-few-of-the-repos-settings)

## 1. Update the docs site's config file

The docs site's config file is `docs/index.html`, which you can find in the repo's docs folder.

In the `docs/index.html` file, update these four lines:

- Line 5: Change `Tool name` to the name of the tool.
- Line 19: Change `Tool name` to the name of the tool.
- Line 20: Change the URL to the new project's URL.

## 2. Update the repository's README

In the repository's README, update the following:

- The repo name
- The repo description
- The repo owners
- Integrations
- The docs site's URL. (It should be https://openpecha.github.io/new-repo-name but with `new-repo-name` changed to the new project's name. You can also find the docs site's URL in the repository's settings in the **Pages** section. You will set it up in [step four](#4-publish-the-site-by-updating-a-few-of-the-repos-settings).)

## 3. Fill out three (or more) content pages

The docs site has three essential pages:

- An [Overview](#overview) that helps users quickly understand the product.
- A [Getting started](#getting-started) guide that covers installation, configuration, and troubleshooting. It also contains a short how-to so users can start using the software within minutes.
- A [Reference](#reference) page to help users perform more advanced tasks with the software.

You will fill out all three of these pages.

There are also two optional pages, which you can add, if necessary, after you finish the first three pages.

- An [Examples](#examples) page to give users code examples to perform common use cases.
- A [Background](#background) page to provide a conceptual guide, background, historical context, etc. that the user might be interested in after they have used the software.

> **Note**: There are also **Help** and **License** pages, but you don't need to update these.

### Overview

This is the homepage for the docs site. You can update it on the README file _inside the docs folder_ in the new repo.

On this page: 

1. Update the title of the page to the name of the tool or project. Example: `# Botok`
2. Write a short overview of the new tool or project. The overview should tell users:
    - What it is/what it does
    - What problem it solves
    - How it works
    - Any other high-level info that users might want to know before using it

#### Good overview examples:

- [Example 1](https://www.atlassian.com/software/jira/guides/more/jira-family#about-the-jira-platform)
- [Example 2](https://rest.sh/#/)
- [Example 3](https://fmartinou.github.io/whats-up-docker/#/introduction/)

> **Note**: Put long or in-depth information on the [Background](#background) page.

### Getting started

The getting started should include prerequisites, installation, configuration, and a short how-to that helps users perform a basic task. By following the steps on this page, users can see how the tool works and appreciate its benefits.  
#### Intro

Describe what this page will include.

#### Prerequisites

- Include the Python version needed
- List other dependencies

#### Installation

Describe how to install the software

#### Configuration

Describe how to configure the software if need.

#### Short how-to (change title)

Write a short how-to section that shows the steps to complete a common task with this tool.

#### Troubleshooting

Add any known issues and solutions here.

#### Good **getting started** examples:

- [Example 1](https://developer.chrome.com/docs/native-client/devguide/tutorial/tutorial-part1/)
- [Example 2](https://www.electronjs.org/docs/latest/tutorial/quick-start)
- [Example 3](https://getbootstrap.com/docs/5.3/getting-started/introduction/)
- [Example 4](https://rest.sh/#/guide)

### Reference

A reference page gives detailed descriptions of specific parts or features of the project. Users look at this page while using the tool, so the page should:

- Be organized into entries, like in a dictionary
- Have a consistent structure, vocabulary, and tone
- Give clear, concise information that fits the description in the overview

It shouldn't:

- Give detailed instructions on how to use the software (put this in the **Getting started** guide)
- Describe the project as a whole (put this in **Overview** or on the **Background** page)
- Describe the concepts or background behind the project (put this on the **Background** page)

#### Examples of good reference pages:

- [Example 1]()
- [Example 2]()
- [Example 3]()

#### Sections

##### Overview

Summarize what this reference article is about.

##### The main section (change title)

Reference articles look different depending on what kind of information you are writing about. The best formats are tables, lists, interactive object-schemas, etc. They allow entries to be shown in a structured way. Most of the time, tables are the best way to show reference information.

This section could also be code-generated.

Change the title of this section.

##### Reference articles

Add links to any reference articles here.

#### APIs and libraries

If the project is an API or a library, include these sections:

##### Overview

Summarize what this reference article is about.

##### Endpoints/library functions

For each endpoint plus method or library function include the following:

##### Resource description

Describe what the API call or library function is used for.

##### Endpoints and methods

Write the endpoint and method such as GET, POST, or DELETE. Or for a library, write the function and method.

##### Parameters

Describe the parameters that users can pass for the endpoint or method to influence the response.

##### Request examples

Include a sample request, showing some parameters configured.

##### Response examples and schema

Show a sample response from the request example above. Also provide a response schema that defines all possible elements in the response.

##### Reference articles

Add links to any reference articles here.

### Examples

The examples page is for providing code samples for various common use cases.

This page is optional. Don't add it until you've completed these pages:

- **Overview**
- **Getting started** guide
- **Reference** page

> **Note**: If you add this page, add it to `_sidebar.md` so users can find it.

### Background

This page is optional. Don't add it until you've completed these pages:

- **Overview**
- **Getting started** guide
- **Reference** page

The background page can include:

- Conceptual overviews that are too long for the overview page in the README,
- The bigger picture and perspective on the tool
- History of similar tools and how this tool is different
- Information about choices, alternatives, and possibilities
- Reasoning and justifications for why the tool is the way it is

> **Note**: If you add this page, add it to `_sidebar.md` so users can find it.

## 4. Publish the site by updating a few of the repo's settings

On your project's GitHub page, navigate to **Settings** > **Pages**.

1. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
2. Set **Branch** to **main**, select the **/docs** folder and **save**.

<img width="672" alt="GitHub pages build and deploy" src="https://user-images.githubusercontent.com/51434640/220822866-b8d804be-ba89-4994-960f-b4ff6b0be8e4.png">
