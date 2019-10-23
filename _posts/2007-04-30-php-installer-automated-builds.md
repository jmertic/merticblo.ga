---
title: "PHP Installer automated builds"
date: "2007-04-30"
categories: [old, php]
---

Just wanted to say thanks to Edin for getting the installer building alongside the normal snapshot builds.

The big thing that got this done was going thru the Feature list and removing those Features without Components that where in the Extensions.wxs file. However, the XPath queries were spotty at best. The clean way of doing this by iterating thru all of the ComponentRefs in ExtensionFeatures.wxs and doing an XPath query on each one would often skip many results, so I had to do the less-than-elegant way and iterate thru the results of getElementsByTagName("Component") for each ComponentRef. At least it works now...

I'm also working on the making the installer work for PHP 6; it's mostly a bunch of %s/php5/php6/g thru the files, so it should be out there relatively quickly.
