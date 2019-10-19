---
title: "Added IIS FastCGI configuration to installer"
date: "2007-09-28"
---

After reading Joe Stanger's [post](http://blogs.msdn.com/joestagner/archive/2007/09/27/fastcgi-for-iis-goes-live.aspx) on the Go Live release of the Microsoft FastCGI Extension, I've added support in the installer for the now in CVS. This should help those on deploying via IIS as it is much better option than CGI ( or ISAPI \*shudder\* ), and the installer will provide automatic configuration of IIS for you.
