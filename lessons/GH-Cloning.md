[comment]: <> (please keep all comment items at the top of the markdown file)
[comment]: <> (please do not change the ***, as well as <div> placeholders for Note and Tip layout)

# GIT Cloning and Forking
***

<span class="oi oi-clock" style="color: orange;">  6 minutes</span> 

[comment]: <> (this is the section for the Note: item; please do not make any changes here)
***
<div style="background: lightgreen; 
            font-size: 14px; 
            color: black;
            padding: 5px; 
            border: 1px solid lightgray; 
            margin: 5px;">

**Note** To reduce complexity of local/remote repositories, the labs will use an easier way for collaborating, just  using the GitHub web interface and remote/origin repository (not local). This will allow you to focus on the content and not on the tooling. However, you can also use a local clone of the repository, and push your changes to GitHub once ready. This will be covered in the next lesson, but not used in the labs.
</div>

## Introduction

In this lesson, you will explore two fundamental concepts in Git: **cloning** and **forking**. Both cloning and forking are essential actions that developers frequently encounter when collaborating on projects using Git repositories. 

Understanding the differences between local and origin repositories is crucial for effective version control and collaboration in Git.

## Git Cloning

### What is Cloning?

Cloning is the process of creating an exact copy of a remote repository on your local machine. This action allows you to work with the repository locally, make changes, and contribute to the project. By cloning a repository, you create a local Git repository with a complete history of all the files and commits present in the remote repository.

### How to Clone a Repository

To clone a repository, you can use the following Git command:

```git clone <remote_url>```


The `<remote_url>` is the URL of the repository you want to clone. For example:

```git clone https://github.com/exampleuser/example-repo.git```

This command creates a local copy of the remote repository in the current directory. The remote URL can be obtained from the repository page on GitHub. You can also use the other options given by the GitHub UI from the **Code** tab of the repository page:

<img src="https://raw.githubusercontent.com/MTT-GH/MTT-GH-SCHOOL/main/lessons/media/clone.png" alt="Clone" style="width:75%; margin: 20px 0px 20px 0px;">


### Cloning Process

When you clone a repository, Git will perform the following steps:

1. **Create a New Directory**: Git creates a new directory with the same name as the repository.

2. **Initialize a Git Repository**: Inside the new directory, Git initializes a new repository.

3. **Fetch Content**: Git fetches all the files and commit history from the remote repository.

4. **Create Remote Tracking Branches**: Git sets up remote tracking branches, such as `origin/main`, to keep track of the remote repository's branches. These branches are used to synchronize your local repository branches with the remote repository one, for example `main` to `origin/main`.

### Collaborating with cloned repositories

When using local(cloned) repositories for collaboration, you will need to synchronize your local repository with the remote repository. This is done by using the following Git commands (others can be used):

- `git pull`: This command fetches the latest changes from the remote repository and merges them into the current branch. It is equivalent to running `git fetch` followed by `git merge`.

When you want to experiment new changes locally and push them to the remote repository, you will need to use the following Git commands (others can be used):

1. Making the desired changes to the local repository.
1. Committing the changes to the local repository, either by using `git commit` or `git commit -a` (to commit all changes), or the UI of your Git client. You could also stage the changes before committing them, by using `git add` (shown in Git Basics lesson).
1. Pushing the changes to the remote repository, by using `git push` or the UI of your Git client.

The following video shows a brief/compact intro to #Git & #GitHub made easy with #VisualStudioCode:

<iframe width="560" height="315" src="https://www.youtube.com/watch?v=i_23KUAEtUM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

## Git Forking

### What is Forking?

Forking is the process of creating a copy of a remote repository to your user account on a code hosting platform (e.g., GitHub or Azure DevOps). Forking is often used when you **want to propose changes to a project but do not have direct write access to the original repository**. 

It enables you to **freely experiment** with modifications without affecting the original project, and **only sharing your updates when/if you are ready**. It gives you the freedom to work on your own copy of a project without affecting the original repository.

[comment]: <> (this is the section for the Note: item; please do not make any changes here)
***
<div style="background: lightgreen; 
            font-size: 14px; 
            color: black;
            padding: 5px; 
            border: 1px solid lightgray; 
            margin: 5px;">

**Forking** is the way people collaborate in Open Source (OSS) projects, as it allows anyone to contribute to a project without the need to be a member of the organization that owns the repository!

</div>


### How to Fork a Repository

Forking a repository can usually be done via the user interface of code hosting platforms. For example, on GitHub:

1. Navigate to the repository you want to fork.

2. Click the "Fork" button in the top-right corner of the repository page.

During the proposed labs, you will be forking the <a href="https://github.com/MTT-GH/MTT-GH-SCHOOL-LABS"> MTT-GH/MTT-GH-SCHOOL-LABS </a> repository to your GitHub user account to learn how to collaborate on content development.

<img src="https://raw.githubusercontent.com/MTT-GH/MTT-GH-SCHOOL-LABS/main/media/upstreamandforkv2.png" alt="Fork" style="width:100%; margin: 20px 0px 20px 0px;">

[comment]: <> (this is the section for the Note: item; please do not make any changes here)
***
<div style="background: lightgreen; 
            font-size: 14px; 
            color: black;
            padding: 5px; 
            border: 1px solid lightgray; 
            margin: 5px;">

**Note:** As mentioned before, labs will NOT use local/cloned repositories, as it makes the process easier, and it is enough for most updates proposed for existing content.

</div>