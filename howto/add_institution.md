---
layout: page
title: How to add your institution
permalink: /howto/add_institution
---

## How to add your institution ##

First of all check that your institution is not already listed. If it is consider editing your institutions page to add new information.

Assuming your institution is not listed then you can add it by cloning the acceleratedcompution.io. github repository and modifying the sites json $institutions.json$ file in the site `./_data` folder. Add you institution name, a image of your university logo (either located in the sites `./static/img` folder or a url to an image on the web) and a url (see next item).

Your institution URL should ideally link to a page on the accelerated computing site. Institution web pages should be placed in the `./institutions` directory. You should copy an existing institutions markdown file which uses the `page` type layout. The `permalink` address in the page header is the link you should specify in the `institutions.json` `url` attribute.

Commit your changes locally and submit a pull request so that your content can be merged with the rest of the site.

Alternatively use the [contact](../contact) page to request that we add your institutions details for you. 

