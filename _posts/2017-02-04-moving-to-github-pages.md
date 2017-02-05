---
layout: post
title: "Moving to GitHub Pages"
date: 2017-02-04
category: News
tags: ModernTLD
---

We've switched between a few hosts for [our website](https://www.moderntld.com/) and we're finally settling on a solution that should be good for everyone. ModernTLD.com and this new news blog are now [hosted on GitHub](https://github.com/ModernTLD) using [GitHub Pages](https://pages.github.com) and behind CloudFlare.

This move offers a few advantages over the old system:

1. Reliability and Independence in hosting
2. Easy editing and distribution
3. Transparency
4. Integrity and Trust

*Are you really independent if you're reliant on GitHub Pages?* This is really a technicality when it comes down to it, we could trivially `git push` to another infrastructure if we ever had any problems with GitHub itself. It's far and away easier to transfer a Jekyll site to another host than a WordPress blog.

This system also allows me to edit the blog as easily as editing a Markdown file (and indeed, all the posts can be found [here in Markdown form](https://github.com/ModernTLD/blog.moderntld.com/tree/master/_posts). And because of the Git based nature of this site, mirrors and distributions can be easily made to make the site more accessible and long lasting than it otherwise would be.

Additionally, this system allows a form of verification that every commit was created by myself, in a manner that a hacker could not reproduce. More on that below.

### Integrity Protection

*End-to-end integrity protection of any distributed information (code, documents, etc) is an extremely important aspect in the digital world, unfortunately way too often ignored by the industry today.* - Joanna Rutkowska, Qubes OS Lead Dev

Now that GPG technology has been [implemented in both GitHub](https://github.com/blog/2144-gpg-signature-verification) and [Git](https://git-scm.com/book/en/v2/Git-Tools-Signing-Your-Work), it's easy to independently verify anything posted to our website or this blog were indeed sent and signed by [myself](https://github.com/JonahAragon) or an authorized ModernTLD volunteer. 

My key can be found at [keybase.io/jonaharagon](https://keybase.io/jonaharagon) and has the following fingerprint:

    D882 B438 57A8 A6B7 80B4 5A37 C309 C927 B8BB F24C
    
(The signing subkey has the ID: `C309C927B8BBF24C`, which will be visible on all GitHub commits)

You can also find my key at the bottom of [wiki.opennicproject.org/JonahAragon](http://wiki.opennicproject.org/JonahAragon) for further verification.

With those three seperate methods of verification, you will be able to assure the [commits posted to this blog](https://github.com/ModernTLD/blog.moderntld.com/commits/master), and the [commits posted to moderntld.com](https://github.com/ModernTLD/www.moderntld.com/commits/master) are from who they claim they are.

Thanks to GitHub Pages and CloudFlare (which provides SSL, caching, speed improvements, and additional reliability), our websites should be more robust against downtime and attacks, and more transparent and open, aligned with the nature of our project.
