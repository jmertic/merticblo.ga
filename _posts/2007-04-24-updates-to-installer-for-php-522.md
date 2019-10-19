---
title: "Updates to the installer for PHP 5.2.2"
date: "2007-04-24"
---

I've reworked the code to configure IIS and Apache to use CustomActions that are included directly in the MSI itself instead of running the installed scripts apacheconfig.php and IISConfig.exe; the big advantage is that I can access installer features and properties directly and now can add uninstaller actions to remove the web server configurations.

Here's the changes:

- Updated Apache configuration; tries to look for directives already existing and comments them out. Also removes the added directives on uninstall.
- Remove IIS configuration on uninstall.
- Force installer to be run by an administrator; should help with Vista issues.
- Other bug fixes ( see [list](http://bugs.php.net/search.php?search_for=&boolean=0&limit=30&order_by=&direction=ASC&cmd=display&status=All&php_os=&phpver=5.2.1&assign=jmertic&author_email=&bug_age=0) )

The next Release Candidate build should have the changes.
