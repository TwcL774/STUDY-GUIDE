# Git

* Git is a version control system that is used to track changes to files and manage projects over time. It is a distributed version control system, which means that it allows multiple developers to work on the same project simultaneously, without the need for a central server or repository.

* At its core, Git is a set of command-line tools that allow developers to manage and track changes to files. When using Git, developers can create a repository (a collection of files and directories) and track changes to the files within that repository over time. They can then share their changes with other developers and merge their changes together in a collaborative and controlled manner.

* Git has a number of key features that make it useful for software development and other projects:

    * Version control: Git allows developers to track changes to their files over time, and to revert to previous versions if necessary.

    * Collaboration: Git makes it easy for multiple developers to work on the same project simultaneously, and to merge their changes together in a controlled manner.

    * Branching: Git allows developers to create branches (separate versions of the project) and to switch between them easily. This makes it easy to experiment with new features or ideas without affecting the main development branch.

    * Distributed: Git is a distributed version control system, which means that developers can work on a project without the need for a central server or repository. This allows them to work offline and makes it easier to collaborate with other developers.

* Git is widely used in the software development industry and has become the de facto standard for version control. It is used by a wide range of organizations and is supported by a large and active community of developers.

## clone

* The git clone command is used to create a local copy of a repository that is hosted on a remote server. When you run git clone, Git will create a new directory and download the entire contents of the repository into that directory. It will also set up a local repository and configure it to track the remote repository, allowing you to push and pull changes between the local and remote repositories.

    * a local copy of a repository hosted on GitHub:
    ```bash
    git clone https://github.com/user/repository.git
    ```
    * a local copy of a repository hosted on GitHub and create a new directory:
    ```bash
    git clone https://github.com/user/repository.git myproject
    ```
    * By default, git clone will create a local copy of the master branch of the repository. Specify a different branch by using the --branch flag:
    ```bash
    git clone --branch mybranch https://github.com/user/repository.git
    ```

## add

* The git add command is used to add new or modified files to the staging area in Git. When you make changes to files in your local repository, Git does not automatically track those changes. Instead, you need to use the git add command to tell Git which changes you want to include in your next commit.

    * add the changes to myfile.txt to the staging area:
    ```bash
    git add myfile.txt or mynewfile.txt
    ```
    * add all modified and new files in the current directory and its subdirectories to the staging area:
    ```bash
    git add .
    ```

## commit

*  The gi commit is used to record of changes made to a project. When you make changes to a project, you can save those changes by creating a commit. Each commit contains a snapshot of the project at a particular point in time, along with a message explaining the changes made in the commit. A commit can include changes to any number of files, and it is useful for tracking the history of a project as it evolves over time. When you create a commit, you are essentially saving a snapshot of the project at that point in time, which you can later refer back to or use as a starting point for future changes.

   * To create a commit, you need to stage your changes first. This involves selecting the changes you want to include in the commit and marking them for inclusion with a commit message.
    ```bash
    git commit -m "comment"
    ```

* After creating a commit, the changes you made will be saved to the project's history, and you can view the commit by using the git log command. This will show a list of all the commits made to the project, along with their commit messages and other details.

## push

*  git push is a command that is used to upload local repository content to a remote repository. When you push changes to a remote repository, you are effectively sending your local commits to the remote repository, where they can be shared with others and incorporated into the project's history. To use git push, you need to have a remote repository set up and connected to your local repository. This is typically done using the git remote command, which allows you to add, remove, and manage remote repository connections. Once you have a remote repository configured, you can use the git push command to send your local commits to the remote repository.

    ```bash
    git push origin main
    ```
    * This would push the local commits to the main branch of the origin remote repository. The origin remote is a special name that is used by default to refer to the original repository that you cloned from.

## remote

* a remote is a repository that is hosted on a remote server and accessed over a network. Remotes are used to share code with others and collaborate on projects. When you clone a repository from a remote server, you create a local copy of the repository on your computer, and you can then use the git remote command to manage connections to the remote repository. The git remote command allows you to add, remove, and view connections to remote repositories.

    ```bash
    git remote add <name> <url>
    ```
    ```bash
    git remote add origin https://github.com/user/repo.git
    ```
    * This would add a new remote repository named origin that is located at the URL https://github.com/user/repo.git. The origin remote is a special name that is used by default to refer to the original repository that you cloned from.

    * to view all remote repositories that are configured
    ```bash
    git remote -v
    ```
## pull

* git pull is a command that is used to download code changes from a remote repository and merge them into your local repository. When you pull changes from a remote repository, you are effectively updating your local repository with the latest changes made by other users.

    ```bash
    git pull origin main
    ```
    * This would download the latest changes from the main branch of the origin remote repository and merge them into your local repository. The origin remote is a special name that is used by default to refer to the original repository that you cloned from.

* When you pull changes from a remote repository, Git will first check to see if there are any new commits on the remote repository that you don't have locally. If there are, Git will download the new commits and merge them into your local repository. If there are conflicts between the remote changes and your local changes, Git will prompt you to resolve the conflicts before completing the merge.

### 1st Setup
```bash
git config --global user.name username
git config --global user.email email@provider.com
```