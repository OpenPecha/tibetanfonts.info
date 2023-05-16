
# Developer's workflow

This is everything you need to do as an OpenPecha developer when you receive and RFC 

## 1. Create an RFC

Review the RFW and [create an RFC](https://github.com/OpenPecha/Requests/issues/new?assignees=&labels=&template=RFC.md&title=%5BRFC%5D) for it. This involves:

1. Understanding the work
1. Considering several possible solutions
1. Understanding the pros and cons of each solution
1. Choosing the best solution
1. Filling out the RFC
1. Submitting it in the [Requests repo](https://github.com/OpenPecha/Requests/) 

See [Everything you ever wanted to know about RFCs but were afraid to ask](article/rfc-about.md) for more about RFCs.

> **Note**: This process should take two days or less.

## 2. Get the RFC approved

1. Let the RFW owners and RFC reviewers know that the RFC is ready for review.
1. Meet on-one-one with each member of the management team to go over the RFC.
1. Integrate management's suggestions.
1. Submit the RFC for management to sign off on.

> **Note**: This process should take three days or less.

## 3. Create a repository for the project

If the approved RFC is for a **new** project:

1. Create a new repo using the [OpenPecha project template for Python projects](https://github.com/OpenPecha/openpecha-project-template) or [this template for projects in other languages](https://github.com/OpenPecha/new-repo-template).
1. Name the repo following [OpenPecha's repository naming conventions](articles/naming-repos.md)
1. Update the repo's README file.
1. Add a short description in the "About" section
1. If the repository has any docs, add them to `/docs` in the root of the repository
1. Transfer the RFC to the new repo.

If the approved RFC is for an **ongoing** project:

1. Update the repo's README file if needed to include information about the new work you are doing.
1. Transfer the RFC to the repo where you will be working.

## 4. Create a GitHub project in the repository

1. Create a GitHub project in the repo.
1. Update your project's description and README.
1. Add a column after **In Progess** and call it **PRs in Review**.

## 5. Convert work phase items into issues

1. Convert each item in the RFC's work phase section [into an issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/creating-an-issue#creating-an-issue-from-a-task-list-item).

## 6. Assign issues to people and add to the project board

1. Assign each issue to yourself or your teammate if you are working as a team.
1. [Add each issue to the project](https://docs.github.com/en/github-ae@latest/issues/organizing-your-work-with-project-boards/tracking-work-with-project-boards/adding-issues-and-pull-requests-to-a-project-board).

## 7. Move the RFC back to the Requests repo

1. [Move the RFC back to the Requests repo](https://docs.github.com/en/issues/tracking-your-work-with-issues/transferring-an-issue-to-another-repository) so management can find it.

## 8. Set up your work environment

1. Clone the repo to your local machine.
1. Make a feature branch.
1. Checkout to that branch.

> **Note**: see also OpenPecha's [coding guidelines](articles/coding-guidelines.md).

## 9. Do the work and create pull requests

1. Move the issue/work phase you are working on to the **In Progress** column of your project board.
1. Work on it and add commits.
1. Go to your standup meetings. 
1. When you finish the issue/work phase, test your work.
1. Make any revisions you need to make.
1. Repeat steps four and five until the code is ready.
1. Move the issue/work phase to the **PRs in Review** column of your project board.
1. Let your assigned reviewers know the PR is ready for them.

## 10. Move to the next issue/work phase

After the PR has been merged:

1. Move the issue to the **Done** column of the project board.
1. Make a next feature branch for the next issue and repeat steps nine and 10 until the RFC is complete.

## 11. Review the process

After you finish all RFC work phases:

1. Review the process with your scrum master and teammate(s),(if any), to see what worked well and what didn't work so well. Use this knowledge to prepare and complete your next RFC.