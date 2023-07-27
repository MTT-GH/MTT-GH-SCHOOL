[comment]: <> (please keep all comment items at the top of the markdown file)
[comment]: <> (please do not change the ***, as well as <div> placeholders for Note and Tip layout)

# What is GitHub?
***

<span class="oi oi-clock" style="color: orange;">  6 minutes</span>

## Introduction

GitHub is a web-based platform for version control and collaboration, primarily used for hosting and sharing code **using GIT repositories**. It provides a centralized location where developers can store, manage, and collaborate on their software projects. GitHub allows developers to track changes in their codebase, work together on the same project, and manage different versions of their code.

[comment]: <> (this is the section for the Note: item; please do not make any changes here)
***
<div style="background: lightgreen; 
            font-size: 14px; 
            color: black;
            padding: 5px; 
            border: 1px solid lightgray; 
            margin: 5px;">

**Note:** GitHub is relying on Git for its Source Control management, but Git is not owned by GitHub. There are many tool that can be used to manage Git repositories, such as Azure DevOps, BitBucket, GitLab, etc...
</div>

Key features of GitHub include:

1. **Version Control:** GitHub uses the distributed version control system called Git. This system allows developers to track changes to their code over time, enabling them to revert to previous versions if needed and collaborate seamlessly with others.

    - **Repositories:** A repository, commonly referred to as a "repo," is a collection of files and folders that make up a project. Repositories can be public, meaning they are accessible to anyone, or private, limited to specified collaborators.

    - **Branching:** Developers can create branches to work on specific features or fixes without affecting the main codebase. Once the changes are tested and ready, they can be merged back into the main branch.

    - **Pull Requests:** When working collaboratively, developers can suggest changes to a repository by creating a "pull request." This allows other team members to review the proposed changes and discuss them before merging them into the main codebase.

1. **Issues and Project** GitHub provides a built-in issue tracking system, allowing developers to create, track, and prioritize tasks, bugs, and feature requests related to the project. It also offers a project management tool that helps teams organize their work and stay on top of their projects.

1. **GitHub Codespaces:** GitHub Codespaces is a feature that allows developers to create a cloud-based development environment for their projects. It provides a fully configured Visual Studio Code environment that can be accessed from anywhere, allowing developers to work on their projects without having to install any software locally.

1. **GitHub Actions:** GitHub Actions is a feature that allows developers to automate their workflows. It provides a way to run custom scripts or commands in response to events such as code commits, pull requests, or issue comments.

1. **GitHub Packages:** GitHub Packages is a feature that allows developers to host and share packages within their organizations. It provides a centralized location where developers can store, manage, and collaborate on their packages.

1. **GitHub Copilot:** GitHub Copilot is a feature that uses machine learning to help developers write code faster and more efficiently. It provides suggestions for code completion, function definitions, and more.

1. **GitHub Pages:** GitHub offers a feature called GitHub Pages that allows users to host static websites directly from their repositories.

GitHub has become a central hub for developers and has significantly contributed to open-source software development, making it easier for people to contribute to various projects and collaborate on a global scale. It has also gained popularity in the industry as a platform for version control, code sharing, and collaborative software development.

In our lesson we will mainly focus on the source control and issue tracking features used to collaborate on content created by WWL content teams.

## GitHub at WWL

WWL has adopted GitHub (together with Azure DevOps) as the main platform to collaborate on content development. 

All the content we see nowadays on platforms like Microsoft Learn or  Skillable are created based on content managed on Git repositories hosted on Azure DevOps or GitHub for source control.

Some of those repositories are public, allowing anyone to contribute to the content, while others are private, only accessible to WWL content teams.

[comment]: <> (this is the section for the Note: item; please do not make any changes here)
***
<div style="background: lightgreen; 
            font-size: 14px; 
            color: black;
            padding: 5px; 
            border: 1px solid lightgray; 
            margin: 5px;">

**Note:** Which repositories will be public/private and how the content is organized may change in the future. The content of the website is based on the actual status of the repositories at the time of writing these lessons. We will adapt it as needed.
</div>

For example, the lab content used for ARB courses (and other modalities)is **public** and hosted in the following GitHub Organization:  <a href="https://github.com/MicrosoftLearning"> MicrosoftLearning GitHub Org </a> . **The focus of this learning journey is showing simple (but impactful) ways to contribute to this content.**

Let´s take the AZ-400 course labs as an example : <a href="https://github.com/MicrosoftLearning/AZ400-DesigningandImplementingMicrosoftDevOpsSolutions"> AZ-400 Labs GitHub </a>

The previous link takes you to the main repository for the AZ-400 course labs. Most repositories will have a similar structure:
<br></br>
<img src="https://raw.githubusercontent.com/MTT-GH/MTT-GH-SCHOOL/main/lessons/media/AZ400_repo.png" alt="Staging Area" style="width:50%;">
<br></br>

- **.github** folder: used for GitHub specific configuration files, such as issue templates, workflows, etc...
- **Allfiles** folder: contains the files used by some of the labs (for example, .NET code used by some lab)
- **Instructions** folder: contains the lab instructions in Markdown format. **This is the folder we will focus on during this learning journey.**
- Other files: files used for other purposes, such as the course outline or the GitHub Page the repositories.

As an collaborator you are mainly going to be proposing changes to the lab instructions or lab files, so you will be mainly working on the **Instructions** and **Allfiles** folders.

Many of these repositories build a **GitHub Page**, which is a static website hosted on GitHub. For example for the AZ-400 course labs, the GitHub Page is hosted here (mostly directed  by shortlinks like aka.ms/az400labs and similar): <a href="https://microsoftlearning.github.io/AZ400-DesigningandImplementingMicrosoftDevOpsSolutions/"> AZ-400 GitHub Page </a>

Additionally, as you can see on the GitHub repository, collaborator are able to report Issues (for problems and feedback), or propose code changes using Pull Requests. We will cover these features in the next lessons.

<br></br>
<img src="https://raw.githubusercontent.com/MTT-GH/MTT-GH-SCHOOL/main/lessons/media/AZ400_issues.png" alt="Staging Area" style="width:50%;">
<br></br>