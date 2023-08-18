[comment]: <> (please keep all comment items at the top of the markdown file)
[comment]: <> (please do not change the ***, as well as <div> placeholders for Note and Tip layout)

# GIT Pull Requests 
***

<span class="oi oi-clock" style="color: orange;">  5 minutes</span> 



## Introduction

A Git Pull Request (PR) is a feature commonly used in collaborative software development workflows. It's a way to propose and manage changes to a codebase hosted in a GIT repository. During the following lesson you will focus on learning about Pull Request workflows for Git repositories hosted in GitHub



Pull Requests can be used to collaborate in the following scenarios:

- Propose changes **between branches in the same repository**. Developers will use the PRs to review changes proposed in a branch (for example, a feature branch) before merging them in a "protected" main branch. 
- Propose changes **from a branch in a fork to the source repository branch**. Used frequently in Open Source or public repositories. A collaborator creates a fork (independent copy of repo to experiment), proposes some changes in a forked repo branch and once tested creates a Pull Request targeting the main branch of the source repo.

### How to create a Pull Request

Focused on the Open Source collaboration scenario (as this is the one used in the labs and also used when collaborating with official lab courseware), the following steps are required to create a Pull Request:

-**Forking**: When working with a shared code repository, you may need to fork (create a personal copy of) the repository to your own account. This allows you to make changes without directly affecting the original codebase.

- **Creating a Branch**: After forking the repository, you create a new branch in your fork to work on a specific feature, bug fix, or improvement. This helps keep your changes isolated from the main codebase until you're ready to integrate them.

- **Making Changes**: You make your desired changes within the new branch. This could involve adding, modifying, or deleting code. It can be done from the GitHub UI or from a local clone of the repository (GitHub UI used in the labs).

- **Committing Changes**: As you work, you commit your changes to the branch. Each commit is a snapshot of the code at a particular point in time and includes a descriptive message explaining the purpose of the changes. **Pushing** will be needed if changes were applied locally (local clone of your forked repo).

    <img src="https://raw.githubusercontent.com/MTT-GH/MTT-GH-SCHOOL-LABS/main/media/upstreamandforkv2.png" alt="Fork" style="width:75%; margin: 20px 0px 20px 0px;">        

- **Opening a Pull Request**: When you're ready to share your changes, you open a Pull Request. This allows you to propose your changes to the original repository. You can also use the Pull Request to ask for feedback or help from other developers. GitHub usually detects branches that got updates and will show a banner to create a Pull Request. You can also create a Pull Request from the **Pull Requests** tab of your forked repository. You should provide a descriptive title and message for the Pull Request, you can even reference issues or other Pull Requests in the message.

    <img src="https://raw.githubusercontent.com/MTT-GH/MTT-GH-SCHOOL-LABS/main/media//update-image-branch.png" alt="Create Pull Request" style="width:75%; margin: 20px 0px 20px 0px;">  

### Pull Request Review


Once a Pull Request is created, other developers can review the proposed changes and discuss them. You can also use the Pull Request to ask for feedback or help from other developers.

- **Reviewing Changes**: Developers can review the proposed changes in the Pull Request, have a conversation using the comments timeline, suggest and approve changes. Most of these actions will be shown in the proposed labs. You could even automate building and testing of the proposed changes using GitHub Actions.
    <img src="https://raw.githubusercontent.com/MTT-GH/MTT-GH-SCHOOL-LABS/main/media/PR-approve.png" alt="Approve Pull Request changes" style="width:75%; margin: 20px 0px 20px 0px;"> 

### Pull Request Merge

Once the proposed changes are reviewed and approved, the Pull Request can be merged by the maintainer. This will apply the changes to the target branch of the Pull Request. 

<img src="https://raw.githubusercontent.com/MTT-GH/MTT-GH-SCHOOL-LABS/main/media/PR-merged.png" alt="Approve Pull Request changes" style="width:75%; margin: 20px 0px 20px 0px;"> 

[comment]: <> (this is the section for the Note: item; please do not make any changes here)
***
<div style="background: lightgreen; 
            font-size: 14px; 
            color: black;
            padding: 5px; 
            border: 1px solid lightgray; 
            margin: 5px;">

**Note:** As mentioned before, labs will NOT use local/cloned repositories, as it makes the process easier, and it is enough for most updates proposed for  content used by MTTs.

</div>
