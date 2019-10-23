---
title: "Updates to the installer for PHP 5.2.1"
date: "2006-12-21"
categories: [old, php]
---

Things that are new to the installer for PHP 5.2.1:

- Support for configuring PHP as an ISAPI module.
- Support for configuring PHP for IIS 7 in CGI and ISAPI modes ( Thanks to [David Wang](http://blogs.msdn.com/david.wang/) for writing a [guide](http://blogs.msdn.com/david.wang/archive/2006/06/24/HOWTO-Install-and-Run-PHP-on-IIS7-Part-3.aspx) on how to do it ).
- Rolling all the IIS Server options into two choices ( IIS CGI and IIS ISAPI ) where the installer will do the right thing based upon the version of Windows you have.
- Some bug fixes ( see the [list](http://bugs.php.net/search.php?cmd=display&status=All&search_for=&php_os=&boolean=0&author_email=&bug_age=0&by=&order_by=id&direction=ASC&phpver=&limit=0&assign=jmertic&begin=0) )

Thanks to everyone who submitted bug reports; you should be seeing those fixes appearing in the upcoming Release Candidates for PHP 5.2.1.
