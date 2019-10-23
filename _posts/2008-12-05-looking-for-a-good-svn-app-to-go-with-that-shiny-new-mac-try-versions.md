---
title: "Looking for a good SVN app to go with that shiny new Mac? Try Versions"
date: "2008-12-05"
categories: [old]
---

Since I use a Mac for my primary development machine at work, I've been looking for a Subversion app with the power and ease of use of TortoiseSVN. I've tried a few different ones, and while they all work for the normal checkout, edit, commit workflow of subversion, I find myself going back to TortoiseSVN every now and then. A few cases for going back include viewing the history of a repository; looking for the full change history of a file, and easily browsing an entire repository. While many of the intergrated clients in Eclipse and other IDEs do this, I prefer a standalone client that doesn't bind me to an IDE since I could be working with a number of different files in the course of a day. And I'm not really a fan of big IDEs anyways ;-).

Enter [Versions](http://versionsapp.com/ "Versions").

The most striking thing to me about Versions is it's intuitiveness and simplicity. All the basic subversion workflow commands are at your fingertips; Checkout, Update, and Commit. A dedicated tab in the main screen shows the recent history of the repository, which is user configurable on how many commits/days you wish to show. There are even dedicated buttons for looking at local changes, history of a file, and running an svn blame to see who changed what line in the file. 

One level deeper we can find some nice advanced functionality. One such thing is reverting back to a particular revision, something every subversion user always has to think twice about on how to do at the command line. You can even edit the svn properties from the right sidebar, which displays information about the selected file. Side-by-side diffing of files is supported, but handled by external programs, such as FileMerge or TextWrangler. You can however intergrate any tool for diffing, check out the [Versions Google Group](http://groups.google.com/group/versions/files "Versions Google Group") for scripts people have submitted.

Versions is also nice since it keeps a check on your checkouts and repositories in real time. It constantly pools your checkouts for changes as well as the main repository. Displaying the number of files you have changed locally, as well as the number of files changed in the repository can be very handy so you know how far behind your checkout is and how many changes you have done locally. In the beta versions this was somewhat buggy, but now it is rock solid.

While Versions is a great tool, I'd love to see the a few things added, namely:

- When a file is in conflict, an option to accept all of the working copy changes and resolve or accept the last revision changes and resolve would be very handy, especially when doing merges.
- In the commit dialog, it would be great to have some word completion, like TortoiseSVN does. Things like filenames and class names in the committed files would be helpful, to reduce spelling errors and typing time.

Big props to the Versions development team on an excellent product!
