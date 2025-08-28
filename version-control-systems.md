# Version Control Systems

The original idea of VCS was to manage tracking changes to documents. The associated meta-data can also be stored; who made the changes, when, and why?&#x20;

In the past when I worked on long-lived documents, at the start of each session I saved previous version with a date stamp. In every document repository, I have a folder called archive. I can go back to every version I’ve ever written of that document, and I can estimate how much work I put in any time and how productive I’ve been.&#x20;

But it’s a manual system and it’s intended for the use of a single person for documents without complex version structure or development branches. And I still do this for important documents! This is a manual _Local Version Control System_, (LVCS) although any system worth that name probably has an underlying database to track things.&#x20;

When I started configuring Unix and DOS based systems, I started keeping script files. My earliest scripts dated back to the 1980s. I started putting in headers and revision numbers. If I could port these to a new Unix system, I could run my scripts and configure systems very quickly.&#x20;

Then the cloud came along!&#x20;

Dropbox let me share to Windows or Linux, all my scripts moved there. But I was still using very manual techniques or [Subversion](https://subversion.apache.org/) on a Cloud share. However, the open-source world has moved heavily to [GIT](https://git-scm.com/) and website services like [GitHub](https://github.com/). These tools are different, although most people seem to associate them as being the same.&#x20;

In this sequence of notes, I will introduce you to GIT and GitHub in both Windows and Linux. My preferred version control has been GIT for several years now.&#x20;

At the start of any collaborative project, I will create a git _repository_ dedicated for that project.&#x20;

After that, I’ll consider opening the project to my collaborators. This is a _Centralized Version Control System_ (CVCS). I can take all this one step further, by mirroring the contents of a CVCS to my local system and working on it independently.&#x20;

Every copy is a full backup of the original.&#x20;

If we set up some tracking mechanisms so that multiple users can make changes and then merge them together to the CVCS, we have a _Distributed Version Control System_ (DVCS).&#x20;

I can add a file, so it becomes a tracked document. When I make a change as a distributed copy, I can stage those changes, selecting which files are to be included. I can commit those changes, permanently recording them in the local database. I can then push the change to the DVCS.
