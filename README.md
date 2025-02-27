[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/8wgCKhpZ)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=18412130&assignment_repo_type=AssignmentRepo)
# se-day-2-git-and-github
## Explain the fundamental concepts of version control and why GitHub is a popular tool for managing versions of code. How does version control help in maintaining project integrity?

Version control is keeping track of project changes and being able save key points of a project which you can check on and return to at any point during development. All your changes, creation, deletion, editing are being monitored.

GitHub is porpular sing it is free, it provide a wide range of features which are easy to use, it intergrates well with git. Some features include, code collaboration with branches and merging, an editor on the platform.

Version control helps with code integrity by providing a way to monitor and view every change being made on the project. This means you will always know what was done and when it was done.

## Describe the process of setting up a new repository on GitHub. What are the key steps involved, and what are some of the important decisions you need to make during this process?

To create a new repostory on github;

On the right side of the top bar in github, there is a + sign with a dropdown arrow, when you click there is a menu with options one being new repository. When you click on it you will be taken to a page where you can create your repository.

Important:

  - The name should not match in of your existing repositories.
  - There's an option to add a dsescription to your repo, which would give information about your repo.
  - Your repo can be public or private, public means anyone can see it, also anyone can fork it, clone, star. This is important if you want collaboration on your repo. A private repo is only visible to you and collaboration isn't possible.
  - A README.md file. This is often used to describe your project, provide documentation, a wiki for users visiting your project. This is a very important file in your project.
  - There's gitignore. This means there are some files that you can choose not to keep track of. What you add in .gitignore will be ignored by git.
  - License. You can choose some liseces, provided on github for your project. Example the MIT license means anyone can use what is in your repo, edit it anyway they want and use it for their own work.

## Discuss the importance of the README file in a GitHub repository. What should be included in a well-written README, and how does it contribute to effective collaboration?

A README file is a form of documentation about your project. It provides a detailed info about what your project is all about and how to use it.
It is useful for collaboration since it gives the objective of the project and anyone visiting the repo for collaboration would know exactly what is being worked on and what is required for the project.

It should contain:
  - The project name
  - A good description telling what the project does.
  - A preview of the project.
  - Instructions on how to collaborate or get in touch with the developer.
  - A list of dependencies if someone is looking to use your program.
  - A detailed manual/instruction on how one can install the program.
  - A help manual on how to use the program and any exceptions for varying systems.

## Compare and contrast the differences between a public repository and a private repository on GitHub. What are the advantages and disadvantages of each, particularly in the context of collaborative projects?

A private repository is one which is visible only to the developer.

It is benefitial if you are working on a personal project which you do not wish to share with anyone. Good for a project with private information.

It is also good if you do not what other people stealing your code.

A dsadvantage about it is that you can't get help from other developers. Since it is only visible to you, no one else can view the repo to offer collaboration.

A public repo is one which is visible to anyone on the internet. Anyone can visit and view the repo to see what you are working on.

An advantage of this is that anyone can visit, see your work and offer collaboration and you can be able to work on the project with them.

Also people can star your repository which will improve your popularity on github.

A disadvantage is that it is not good if you are working on a personal project with personal information.

## Detail the steps involved in making your first commit to a GitHub repository. What are commits, and how do they help in tracking changes and managing different versions of your project?

The steps of you first commit:
  1. In your folder containing your work, write; `git init` this will initialize git.
  2. Then write; `git add .` this will add everithing in that folder to git and in a stage waiting to commit.
  3. Then; `git commit -m "Initial commit"` this will commit the changes and the commit message will be *"Initial commit"*.
  4. Then; `git branch -M main` this will set the main branch
  5. Then; `git add remote origin "https://github.com/example.git"` this will be the link to your repo on github where your project will be stored.
  6. Then; `git push -u main` this will push your code up to your github repo. This will be on the main branch.

Commits are like savepoints in a game, they are like a mark for a certain point in your development process. When you commit, you add a commit message which often describes the changes you've just made. With that you can easily revisit that point.

## How does branching work in Git, and why is it an important feature for collaborative development on GitHub? Discuss the process of creating, using, and merging branches in a typical workflow.

Branching is creating another branch separate from the main branch. This allows you to make changes to the project without affecting the main branch/project. If you are satisfied with the changes in that branch you can merge it to the main branch.

Branching is especially useful for collaboration. Different teams will have different branches from the main, allowing them to work on their specific areas and after they are done, they all merge their brances to the main branch.

To create a branch, we use: `git branch "branch-name"` and use: `git checkout "branch-name"` to move into that branch.

Alternativelty you can use `git checkout -b "branch-name"` which will both create and move you into that new brance.

When in the created branch, you can perform changes and commit them. Then when you are stisfied with the changes, you can merge the branch into the main branch.

To merge to the main branch, we use: `git checkout main` to move back to the main branch. Then: `git merge "branch-name"` to merge the other branch to the main branch.

After merging you can delete the other branch using `git branch -d "branch-name"`

## Explore the role of pull requests in the GitHub workflow. How do they facilitate code review and collaboration, and what are the typical steps involved in creating and merging a pull request?

A pull request is a way for another developer to offer assistance on another developers project on github.

To perform a pull request
  1. Fork the repo on github. This will add the repo to your own github and you can keep track of the changes from the forked repo.
  2. Clone the forked repo into your machine.
  3. Create branch which will contain the changes you want to make.
  4. In that branch you can perform editd, do git add and commit the changes.
  5. You can then push the branch to your github fork and then on github you'll have the option to perform a pull request. You'll add a message to the pull request and send it. Then wait for the developer to accept your pull request.

## Discuss the concept of "forking" a repository on GitHub. How does forking differ from cloning, and what are some scenarios where forking would be particularly useful?

Forking is when a github version of the original repo is created on your own github. The forked repo will keep track of the main repo and inform you of the changes. Unlike cloning is when you download that repo onto your local machine.

Forking is useful when you want to collaborate on another developers project. This will help in performing full requests.

Also it is useful if you want to stay up to date with a certain project.

## Examine the importance of issues and project boards on GitHub. How can they be used to track bugs, manage tasks, and improve project organization? Provide examples of how these tools can enhance collaborative efforts.

This is a way for people who are using your program to report the errors they face when using it. Reported issues can then be worked on and you can provide the solution. Other users with the same issue can visit the issues page and see how the error was solved.

Other developers can also visit the issue page and if they can solve the error they will solve and perform a pull request.

## Reflect on common challenges and best practices associated with using GitHub for version control. What are some common pitfalls new users might encounter, and what strategies can be employed to overcome them and ensure smooth collaboration?

New users to github can be overwhelmed with all the available options.

They can find it hard to keep track of all the comands used.

To help in this, their should be a wiki, a form of cheatsheat with detailed instructions and examples of github comands and features.
