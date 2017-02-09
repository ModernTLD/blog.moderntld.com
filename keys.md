---
layout: page
title: GPG Keys
permalink: /keys/
---

GitHub contributors, editors of [moderntld.com](https://www.moderntld.com/), and authors of this blog all use GPG keys to sign their commits (starting from Feb. 4, 2017). This is very important because it allows you to verify that the changes made to our websites and code repos were made by trusted representatives, as opposed to a theoretical GitHub breach or account hijacking.

The sections listed below display key info for all people who are members of the [@ModernTLD](https://github.com/ModernTLD) group on GitHub. This page is a work in progress (we hope to include everyone soon).

*How do you check Git commit signatures?*

On the commits page of any GitHub repository, signed commits will show a "Verified" badge, which lets you know the commit in question is signed, and will show you the GPG fingerprint of the key used to sign said commit.

For example, on the [Git commits page](https://github.com/ModernTLD/blog.moderntld.com/commits/master) for this website:

![](/assets/images/gpg.png)

### Jonah Aragon

**Prior to Feb. 8th**, commits by myself, [@JonahAragon](https://github.com/JonahAragon) were signed with [my master key](https://raw.githubusercontent.com/JonahAragon/JonahAragon.github.io/master/keys/jonah-master.asc) which has the fingerprint `C309C927B8BBF24C` on all GitHub commits.

This master key **should still be used for encrypted communications** (emails, etc) but no longer signs any future GitHub commits.

This master key in full is linked above, and is also accessible at [keybase.io/jonaharagon](https://keybase.io/jonaharagon).

Further verification: [Twitter](https://twitter.com/JonahAragon/status/828617198461665281) [OpenNIC Wiki](http://wiki.opennicproject.org/JonahAragon)

**After Feb. 8th**, my GitHub commits are signed by a separate [GitHub signing key](https://raw.githubusercontent.com/JonahAragon/JonahAragon.github.io/master/keys/jonah-github.asc).

This key is *signed* by my master key for authenticity, but for security reasons is kept separate for GitHub signing purposes *only*. (If you need to send me encrypted communications please use [my master key](https://raw.githubusercontent.com/JonahAragon/JonahAragon.github.io/master/keys/jonah-master.asc)!). The GitHub key in question will show the ID `0209F0BBFEEB8CEF` in GitHub commits.

```
pub  4096R/FEEB8CEF  created: 2017-02-05  expires: never       usage: SC
                     trust: ultimate      validity: ultimate
sub  4096R/2433E176  created: 2017-02-05  expires: never       usage: E
[ultimate] (1). Jonah Aragon (GitHub Signing Key) <jonaharagon@gmail.com>

gpg> check
uid  Jonah Aragon (GitHub Signing Key) <jonaharagon@gmail.com>
sig!3        FEEB8CEF 2017-02-05  [self-signature]
sig!         B8BBF24C 2017-02-05  Jonah Aragon <jonah@jonaharagon.com>
```

### Joseph Marsden

**Effective from Feb. 9th onward**, commits by me, [@CitadelCore](https://github.com/CitadelCore), are signed by my master GPG key.

```
pub  4096R/3CD0AB23  created: 2017-02-03  expires: never       usage: SC
                     trust: ultimate      validity: ultimate
sub  4096R/0D22CE92  created: 2017-02-03  expires: never       usage: E
[ultimate] Joseph Clayton Marsden (CitadelCore) <josephmarsden@towerdevs.xyz>
```

[This key](https://keybase.io/CitadelCore/pgp_keys.asc) can be found at [keybase.io/citadelcore](https://keybase.io/citadelcore) for further identity verification.
