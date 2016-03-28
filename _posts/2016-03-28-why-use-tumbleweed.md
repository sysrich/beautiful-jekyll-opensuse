---
layout: post
title: Why You Should Use Tumbleweed
date: '2016-03-28 19:05:02'
---
People often ask me why they should use [openSUSE Tumbleweed](http://www.opensuse.org) and how it compares to other distributions like Fedora or Ubuntu. The fact is Tumbleweed is actually rather hard, if not impossible to compare to Linux distributions like Fedora or Ubuntu

Both are 'traditional', released-based distributions. They build it carefully over a few months, they ship it, and they then cautiously patch things (often keeping those changes as small as possible, backports, etc) to keep it secure/usable for their users over their chosen lifespan

If you're interested in an openSUSE like that, we have [Leap](http://www.opensuse.org), and I believe Leap to be better than Fedora and Ubuntu for a whole bunch of reasons, starting with the fact that Leap has an Enterprise codebase (SUSE Linux Enterprise to be exact) at it's heart with the openSUSE Project building a fully-fledged community distribution ontop of it.

Today I want to talk about Tumbleweed  
While Leap aims to be rock-solid, Tumbleweed rolls

It's more like Arch and Gentoo in that regard. Tumbleweed today contains the latest packages of every software stack that has been packaged by the openSUSE Project. Latest kernel, libraries, desktop environments, everything in Tumbleweed can and does change regularly

But, unlike other rolling distributions, Tumbleweed does it smarter

# Built Correctly
Tumbleweed is built like a 'traditional' distribution. All packages in Tumbleweed are built together as a cohesive distribution, and shipped together as a cohesive distribution. If a new package in checked in that potentially can invalidate another package (eg. new glibc, new libraries, new kernel, etc) then the dependant packages are rebuilt, just like traditional distributions.

But where as traditional distributions take days, sometimes weeks to do such, we do it in hours, because we have the Open Build Service

* You can learn more about [Open Build Service HERE](http://openbuildservice.org/)
* You can see, and use the [openSUSE Build Service](http://build.opensuse.org) for free, today

This produces a 'snapshot'. At this point a traditional distribution would probably call this a 'release candidate', an ISO and a set of repositories with all the software built and ready for testing.

>Most distributions take weeks to produce coherently built and tested disk images & repositories. Tumbleweed does it about 5 times a week

# Tested Well
But building is only half the story. A good distribution needs to be tested. A good rolling distribution needs to be tested quickly. Arch and Gentoo rely on manual testers and purposefully delaying the inclusion of packages in their main repos in order to give people time to test stuff. openSUSE has openQA

Before any human being is allowed anywhere near a snapshot, openQA tests that snapshot over 100 times across four different hardware architectures (i586, x86_64, ppc64, and aarch64)

These are not artificial 'some developer writing some code to poke around some APIs' kind of tests

openQA actually does proper *real-world* scenarios. Installations, upgrades, dual booting, encrypted LVM, kde, gnome, xfce, live CD's, network installs.  
You name it, we test it. And if we don't test it well enough we want to and you can contribute tests as everything in [openQA is 100% open source](http://os-autoinst.github.io/openQA).

![There are far many results to show in this blog post](/pics/openqaresults.png)  
[Just take a look at the openQA results for a recent Tumbleweed snapshot for example, just to give you an idea](https://openqa.opensuse.org/tests/overview?distri=opensuse&version=Tumbleweed&build=20160321&groupid=1)

Again, these aren't some kind of artificial 'some fancy coder wrote a robot that can mash buttons in the right order' tests. openQA can actually **see** the screens it is testing.

It uses openCV and a library of reference screenshots (with areas of interest selected to allow openQA to ignore things we don't care about) which we call 'needles'

So every test checks that every screen looks the way we want it to look for users. Every function that is tested presses the same keys and clicks on the same mouse buttons that a user would, and then openQA confirms that piece of software behaves in the way it has been taught to expect

openQA does this for every step in installations & upgrades.  
openQA checks all the core console commands, systemd, zypper, YaST in ncurses mode, curl, vim, firewall, ssh, etc etc  
openQA then logs into the desktop environment of choice (GNOME, KDE, lxde, xfce, etc) and checks graphical applications. Is gedit working? firefox? thunderbird? libreoffice? inkscape? gimp? etc etc

And it does this all in dozens of different scenarios, over and over again, in parallel across many VMs and machines.

We even do extra testing on incoming package submissions, so many cases we catch things before they get anywhere near a snapshot, and our developers get nice fast feedback about their otherwise potentially destructive change. Yes, we have implimented Continuous Integration for distributions, and if you were using [OBS](http://openbuildservice.org) and [openQA](http://os-autoinst.github.io/openQA) you could be doing it too.

# Delivered Quickly
1000's of tests, over 100 scenarios...and with our current hardware (thanks [SUSE](http://www.suse.com)!) a full snapshot gets tested in about 3 hours

And if it passes, it ships, **automatically**.

Most distributions take weeks to produce coherently built and tested disk images & repositories  
Tumbleweed does it about 5 times a week

And a 'quiet' week can consist of approx new/updated 150 packages and a new kernel..  
A normal week is double, if not triple that, and it's moving faster and faster..

All that extra work doesn't get in the way. We often beat other rolling distributions into delivering tested versions of KDE Plasma and GNOME, because we can test them quicker and ship them with a certainty that nothing breaks.

That's not universally true though, good testing finds bugs, those bugs need to be fixed, so if you ever notice something taking longer than you'd like, it's often a sign that we could do with more contributors helping Package that particular software. [You can learn how to contribute to Tumbleweed HERE](https://en.opensuse.org/openSUSE:Factory_development_model).

# Trusted by More and More
Most of what I describe above was implimented after July 2014 and culminated in the ['merger' of Old Tumbleweed and Factory in November 2014](https://news.opensuse.org/2014/10/24/tumbleweed-factory-rolling-releases-to-merge/)

Since then, the adoption rate of Tumbleweed has been nothing short of astronomical.. ![Look at those numbers](/pics/Tumbleweedstats.png)

If [public numbers are to be believed](https://www.archlinux.de/?page=UserStatistics) Tumbleweed might already be larger than 'more famous' rolling distributions. Whether or not that's true doesn't change one fact - **We want YOU to try Tumbleweed**

And you'll be in good company. Not only amongst those users, but companies like [SoftIron](http://softiron.co.uk/) who ship Tumbleweed on their Overdrive 3000 64-bit ARM servers, and [Fujitsu](http://ts.fujitsu.com) who offer Tumbleweed as their chosen community Linux to customers with Skylake hardware.

I may be biased, but Tumbleweed is the only rolling distribution I'd recommend to _any_ Linux enthusiast as their daily driver.

If you care about Linux, you want the latest packages, but you only want them when they actually work, Tumbleweed is the best choice, bar none.

And anyone who disagrees with me is welcome to join the [openSUSE Project](http://www.opensuse.org), find us on [opensuse-factory@opensuse.org Mailing List](https://lists.opensuse.org/) and help make it even better ;)

*NOTE: This blog post started as a response to a [Reddit Post](https://www.reddit.com/r/linux/comments/4bytfz/thoughts_please_on_opensuse_tumbleweed/). Thanks to the OP for the inspiration!*
