# GIT

Linux kernel development was informal from c. 1991 onwards, with patches being passed around in various archive formats. From c. 2002, these patches were maintained in a proprietary distributed version control system; BitKeeper. In 2005, free access to this DVCS was removed and legend has it that Torvalds wrote GIT in 10 days!&#x20;

GIT is based on a repository (or repo), a file system with meta-data to track versioning. Each time a change is committed, GIT takes a snapshot of what the file system looks like; any file which has been changed is stored, and file which is unchanged is saved as a link to the previously saved version.&#x20;

All operations are local, you only need to be connected to the Internet to update a central repo.

Integrity is built into GIT; every file is fingerprinted using a SHA1 hash. A hash is a unique fingerprint of a file, changing any character will change the hash value.&#x20;
