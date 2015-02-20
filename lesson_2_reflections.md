Lesson 2 Reflections
=======================

- What happens when you initialize a repository? Why do you need to do it?
	When you initialize a repository, it essentially creates a "folder" within git. It needs to be done so that changes can be tracked and commits can be made. 

- How is the staging area different from the working directory and the repository? What value do you think it offers?
	The repository contains the most recent committed versions of the files inside it, and the working directory is the local/on-disk copy of the files that a developer works on. The staging area only contains the changes made to the files in the working directory, which are accumulated in a commit to the actual repository.

	It offers the ability to prepare and finalize the files that you want to commit to the repository, before you actually have to commit. It also allows you to separate the files you plan on editing, so that you can commit only certain files or certain parts of files. This allows you to deliver more logical commits that are separated by features or some other metric.

- How can you use the staging area to make sure you have one commit per logical change?
	You can use the staging area to only commit certain files or parts of files. This lets you only commit the relevant data for a given feature and separate your commits by features/logical changes. 

- What are some situations when branches would be helpful in keeping your history organized? How would branches help?
	Branches help you keep your history organized by allowing a developer to see the order in which commits were made and by whom. This can help a person keep track of what version of the program a given person may be working with, as well as keeping track of how the program is forked and merged back together. 

	Branches are also useful in that they can be used to separate the different versions of a program in a Kanban flow. As a feature moves from development to testing, the commits made to the development branch can then be merged into the testing branch for QA to work with. Then from the testing branch, it can be merged into pre-release, which is eventually merged into the master/release branch that the client/user uses. 

	Branches are also useful for literally branching off a project to fulfill a different function, or for use in an application

- How do the diagrams help you visualize the branch structure?
	The diagrams visualize the commits made to a branch as well as the order they were made in. It also shows someone at what point a fork forms, and at what points a branch merges back. Since it shows the different forks and merge points, you can also see at what branch a commit was made and the context of a given commit.

- What is the result of merging two branches together? Why do we represent it in the diagram the way we do?
	Merging two branches together combine the contents of the two branches into a single branch. If there are file conflicts, it usually opens a diff and allows for final changes to be made to resolve the conflict and help the merge along. 

	We represent it in the diagram the way we do because it is effectively a new commit where the differences between two branches are put together to form a new branch. 

- What are the pros and cons of Git's automatic merging vs. always doing merges manually?
	Git's automatic merging is convenient because it automatically combines the branches for files that don't conflict and thus don't cause obvious issues with each other. It speeds the process of merging up considerably, compared to merging manually. This is because to merge two branches manually, you have to go through every single file, which can be tedious. The downside to Git's automatic merging is that it can potentially introduce bugs that are not obvious and entirely environment-based. Another downside is that Git cannot handle file conflicts, so they still have to be done manually. 