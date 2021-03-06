Lesson 1 Reflections
====================

- How did viewing a diff between two versions of a file help you see the bug that
was introduced?

    Viewing a diff lets you easily see what has been added/removed from a file. This makes the changes stand out like a sore thumb, and can reveal the root cause of any bug, whether it is due to a typo, a missing semicolon on a new line, variables that have been poorly refactored, or poor logic in new ode. 

- How could having easy access to the entire history of a file make you a more
efficient programmer in the long term?

	It allows you to see the progression of features. It also allows you to go back and see a previous implementation of a given feature, and lets a developer compare the benefits of the different implementations. It also lets you see what the other developers on the same project are working on. It also allows you to restore previous versions in case of a massive issue

- What do you think are the pros and cons of manually choosing when to create a
commit, like you do in Git, vs having versions automatically saved, like Google
docs does?

    It makes commits more intentional. You can specify exactly what has been changed in a given commit using the commit message, and it allows a person to revert to specific commmits and see the progress made. 
    Automatic saving makes it less likely that data can be lost from any issues
    It is easier to keep track of different versions using commits
    Manual saving and commits encapsulate new features within a given commit, when done properly.

- Why do you think some version control systems, like Git, allow saving multiple
files in one commit, while others, like Google Docs, treat each file separately?

    Because they try to work towards two completely different niches. Google Docs focuses on document creation, in which a person generally only works on one or two documents at a time, and they operate independently of each other. Due to this independence, they are treated separately and saved separately. 

    Compare this to Git, where adding a feature or making changes involves creating and editing multiple files that interact and rely on each other. Saving multiple files in a single commit allows new features being saved to be encapsulated within a commit. It groups together the changes that belong together. 

- How can you use the commands git log and git diff to view the history of files?

    `git log` allows you to view all the commits that have been made, the date each commit was made, the author of each commit, the message associated with that commit, and the hash/checksum/thing of the commit.
    `git diff` allows you to view the changes made to a file, and view the differences between two given versions of the file (whether its the current and the previous version, or two older versions)

- How might using version control make you more confident to make changes that
could break something?

    If changes that I make break something important, I can use version control to revert back to a previous, known working commit. 

- Now that you have your workspace set up, what do you want to try using Git for?

    I'm currently using git for this reflections document, as well as the StegoProject for my group. I am not, however, making proper use of branches because I'm lazy. 