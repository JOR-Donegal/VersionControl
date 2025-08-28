# Scope and Requirements

Sometimes when I’m working on academic papers with collaborators, we use tracking in Word. It can be madly complicated, as we all make changes, put in notes, change the changes, etc. We need something better for complex documents and projects.&#x20;

In such a system, we can see

* What changes were made and keep track of the changes in the long term
* Who made changes (blame)
* When they were made

And we can go back to earlier versions.&#x20;

What is the scope and functional requirements for a versioning system?&#x20;

Firstly, I need my files to be kept in a location where they can be accessed by me and by others. In a revision control system, a starting point is to create a repository or repo There is an expression; “single source of truth”. You can’t have multiple, unconnected versions of the same project. If the versions are unconnected, that’s a different project.&#x20;

If we _clone_ a repository, we create a copy, but we could keep it synchronized with the original. You can clone any repository which has public access or which you have authentication to access.&#x20;

For any public repository, you could create a _fork_, that is a copy of that repository in your own account; everything. From the time you fork the repository, it is a separate strand of development. If the owner of the original repo performs other commits, they will not show in your fork. Similarly, if you perform commits, they do not show in the original repo. After an initial release, the repository could hold bug fixes, new versions, etc.&#x20;

Secondly, we would need to be able to track any files in the repo considering collaboration between team members.&#x20;

Finally, we should be able to see who did what and when, we call this _blame_. We need the ability to roll-back changes which might have proved problematic, accountability.&#x20;

Although we can track files individually, for complex projects we track the project as a whole and files are specifically subject to revision control. Where a user needs to edit a file, it is checked out and made available to that user as a working copy. When the user is satisfied with the edit, they can commit the file by saving it and then checking it in, back into the repository.&#x20;

Each time a commit occurs, it is identified by a unique revision number and the most recent version is the HEAD.&#x20;

If multiple people are working on the same dataset, then they may produce conflicting edits, and any revision control system will require a protocol for _merging_ changes. Thinking of this in terms of graph theory, the version control system can be viewed as a directed tree with multiple parallel lines of development which may branch and later merge. Multiple users can share a version control system, but it is possible to have conflicts, and, in this case, manual intervention may still be required during merge operations.
