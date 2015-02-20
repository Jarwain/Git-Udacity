Lesson 3 Reflections
=====================

When would you want to use a remote repository rather than keeping all your work local?

    You'd want to use a remote repository when you are working with people other than yourself. It makes it easier to collaborate with others and make larger/different changes to the project. If all of your work is local, other people on the team can't exactly fork and use that efficiently or effectively. 

Why might you want to always pull changes manually rather than having Git automatically stay up-to-date with your remote repository?

    Another person working with you on your remote repository might push a change that would:
    - Break a feature you are currently working on
    - Overwrite a feature you are currently working on
    - Break some other part of the project causing the build to fail and preventing you from testing your own work
    If Git automatically stays up-to-date with your remote repository, these changes will directly affect your work. However, pulling changes manually allows you to time it so that you can, say, pull after you are completely done with the feature, and when the build is in a working state. It also lets you deal with file conflicts on your own time instead of every time git tries to auto-sync, which can be distracting/annoying. 

Describe the differences between forks, clones, and branches.  When would you use one instead of another?

    Clones are a complete copy of a repository. It generally creates a new repository to be edited/changed locally. You'd use clone to create a copy of an existing repository locally, or to create a fork of a different repository.
    Branches are a split off of a repository that contains commits relevant for a given feature, sprint, or development cycle. They are used by the main developers of a project to make changes to the project effectively, since they have read/write access to the project. 
    Forks are a more conceptual thing. A fork of a repository is effectively a branch of the project, except it was created through a clone and is, in a sense, its own project. Forks are usually created in one of two scenarios. A fork of a program could be a completely new project started by some developers who were not happy with the direction that the original project has taken, and thus uses the original project as a base that is modified. A fork of a program could also be a branch of another project, created by a developer who does not have write access to the original project and thus has to make his own fork. This is the scenario popular on github: a developer forks a project to make changes/add features, then submits a pull request to have their fork merged back into the project. 

What is the benefit of having a copy of the last known state of the remote stored locally?

    Having a copy of the last known state of the remote stored locally gives you the current (hopefully working) build of a project/repository. It gives you an up-to-date base to build new features on top of, while minimizing the amount of worrying that needs to be done when merge-time comes around. It also gives you context, in case another developer makes different changes to the project, you can compare the updated version of the project to the one you have locally, and see if there may be any conflicts between it and what you are working on.

How would you collaborate without using Git or GitHub?  What would be easier, and what would be harder?

    If I had to collaborate without using Git or Github, I have a couple other options. 
    - I could learn a different version control system such as SVN
    	- It would have a learning curve, but be equally as easy to deal with post-curve

When would you want to make changes in a separate branch rather than directly in master?  What benefits does each approach have?

    You make changes in a separate branch to encapsulate a feature more effectively than any commit. Encapsulation in commits are good for small changes that collaborate to establish a feature, but encapsulation in branches allows one to work on a feature fully independently of other who are working in their own branches on different features. This is largely more efficient/effective than constantly committing to master, just because it minimizes the amount of conflicts and issues that may arise from development.m 

    Working directly in master is only acceptable if you are the only developer working on the project, and even then it is considered extremely sloppy.