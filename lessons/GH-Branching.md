[comment]: <> (please keep all comment items at the top of the markdown file)
[comment]: <> (please do not change the ***, as well as <div> placeholders for Note and Tip layout)

# GIT Branching
***

<span class="oi oi-clock" style="color: orange;">  3 minutes</span> 

## Introduction

[comment]: <> (this is the section for the Note: item; please do not make any changes here)
***
<div style="background: lightgreen; 
            font-size: 14px; 
            color: black;
            padding: 5px; 
            border: 1px solid lightgray; 
            margin: 5px;">

**Note** The concepts shown in the following lessons (branching, cloning/forking and PRs) are not specific to GitHub, but are common to all GIT-based source control systems.
</div>

Branching is a core concept in GIT. It allows you to create multiple branches for your code repo and work on them independently. This is useful when you want to add a new feature or fix a bug without affecting the main codebase. Once you are done with the changes, you can merge the branch with the main codebase.

Based on this idea, many branching strategies have been developed, such as GitHub Flow, GitFlow, and others. Here you can find a common branching strategy used by many Microsoft product teams, such as the Azure Devops one : [How Microsoft develops with DevOps](https://learn.microsoft.com/en-us/devops/develop/how-microsoft-develops-devops)

As an MTT , you will mostly use a simple feature branching strategy (trunk based development) that works the following way:

![Feature Branching](https://raw.githubusercontent.com/MTT-GH/MTT-GH-SCHOOL/main/lessons/media/featurebranching.png)

- **Main** branch : This is the main branch of the repository (the trunk). It contains the latest **stable version of the codebase, the one ready for release at any time**. As a maintainer you usually **protect the main branch** so that changes can only be merged through Pull Requests.
- **Feature** branch : This is a temporary branch that is created to work on a new feature or fix a bug. It is created from the main branch and merged back into the main branch once the changes are tested, mostly using a Pull Request. As a contributor, you will create a feature branch from the main branch, work on the changes, test them, and then merge it back to the main branch through a Pull Request.


## Branching in GitHub 

You can view, edit and create branches in GitHub from the **Code** tab of the repository page, clicking on the default branch dropdown:

![Create branch](https://raw.githubusercontent.com/MTT-GH/MTT-GH-SCHOOL/main/lessons/media/createbranch.png)


[comment]: <> (this is the section for the Note: item; please do not make any changes here)
***
<div style="background: lightgreen; 
            font-size: 14px; 
            color: black;
            padding: 5px; 
            border: 1px solid lightgray; 
            margin: 5px;">

**Note** Branches can also be created from a local (clone) repository , and push them to GitHub once ready. This will be covered in the next lesson, but not used in the labs, as we are going to use an easy approach to create branches and work directly in GitHub (no local clone/repo needed).
</div>

When you are editing a file using the GitHub editor , you will see the chosen branch name on top of the file, that is the branch we commits are going to be pushed to:

![edit file](https://raw.githubusercontent.com/MTT-GH/MTT-GH-SCHOOL/main/lessons/media/editfile.png)

