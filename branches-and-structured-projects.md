# Branches and Structured Projects

You will already have seen the term _branch_ if you have done any of the exercises and you will have seen it on GitHub.

<figure><img src=".gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

The branch **main** was created when we setup the repo, and when we pushed from the local machine, we pushed the remote origin, to the branch main. We have a standard approach with branches when we are doing code development.

<figure><img src=".gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

I marshal my work on the dev branch.&#x20;

Once the code functions, I can push it to the test branch for extensive testing.&#x20;

Once the code passes QC checks and tests, I could merge it into the main branch, and it becomes production code.&#x20;

When I’m developing, each task will have a start and an end, for example a new feature or a bug fix. Each change I make will originate on its own branch and be merged into the dev branch.

<figure><img src=".gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

Most commits should be on dedicated feature or bug fix branches, this is where all the editing should be done. These are then merged to the test branch.&#x20;

As work is tested, it can be merged from test to main. The closer we get to the master branch, the more we should see merges, not commits. In GitHub we have merges and pull requests, which we use to combine these branches.
