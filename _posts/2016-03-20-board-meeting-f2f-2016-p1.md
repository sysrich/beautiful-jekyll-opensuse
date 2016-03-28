---
layout: post
title: openSUSE Face-to-Face Board Meeting 2016 Minutes - Part 1/3
date: '2016-03-20 16:20:00 +0100'
categories:
- Board
---
18th-20th March

Present:

* Richard Brown - Chair
* Michal Hrušecký
* Kostas Koudaras
* Tomas Chvatal
* Gertjan Lettink
* Bryan Lunduke - Extra special thanks goes to Bryan for attending
via video conference at ridiculous hours in his local timezone after
urgent personal matters kept him from attending the meeting in person.

As this years Board Meeting Minutes are so long, they are split into 3 sections

* Meetings - Covering the meetings the Board had with various SUSE
executives, managers, and engineers.
* General - Covering the general agenda items/day-to-day issues
* Strategy - Covering the 'big picture' issues the Board discussed

This email is Part 1, containing meeting minutes of meetings with SUSE

Part 2 is available [HERE]({% post_url 2016-03-20-board-meeting-f2f-2016-p2 %})

Part 3 is available [HERE]({% post_url 2016-03-20-board-meeting-f2f-2016-p3 %})

## Meetings

### Meeting with openSUSE Release Manager - Ludwig Nussel
The Board met the new openSUSE Release Manager - Ludwig Nussel

He shared the following tentative information about the planned
release for Leap 42.2:

* Leap 42.2 will be based on SLE 12 SP2 and their release scheduled are
'aligned' (ie. They will be developed together, but not necessarily
release together)
* Target release date for Leap 42.2 is 1st week of Nov 2016.
Expected to have an updated systemd, GNOME, Qt, kernel all inherited
from SLE 12 SP2
* KDE of course will want to upgrade from 5.5, expected 5.6, discussions
underway about what upgrade policy will make sense for the lifespan of
Leap 42.2
* We don't expect X will be updated, which will mean 42.2 will have the
same version as 42.1, which is newer than the version in SLE 12 SP1 or
expected in SP2

Leap 42.2 will start with a base of Leap 42.1, with packages updated
from that point. The process for contributing to Leap 42.2 needs
explanation

We discussed the shape of how we'd like to see the wiki. 
We all agreed want to see a big tidy up. Many of the Portals have
little benefit and serve little purpose. We want to see the namespaces
removed/flattened to help the search

* Tumbleweed deserves a Portal. Questions the page must answer include
"What is Tumbleweed?" "Why use Tumbleweed?" and "Why might Leap be
better for you?"
* Leap is similarly important, needing to answer the questions "What is
Leap?" "Why use Leap?" and "Why might Tumbleweed be better for you?"
* Packaging Polices and the Factory process are other 'key' pages which
must be preserved, polished, and refreshed during any wiki cleanup
* Team pages would be 'nice to have' but many Team pages are currently
woefully out of date. We would like to see a solution investigated
where the wiki team page is inherited from a devel project

We discussed the idea of forming a "Release Team" with specific roles
that are responsible for ensuring that key parts of the Release
process are carried out
 
Obvious roles include "Website coordinator" to ensure the website is updated.
 "Wiki Coordinator",  "Marketing Coordinator",  "Test Coordinator",
"Translation Coordinator" are other obvious roles

 These people would not necessarily be responsible for doing the work,
but for coordinating with Ludwig and ensuring that the work gets done
by someone.
 
**AI:** Ludwig to mail the Board with any other "Roles" which are
expected to be needed

**AI:** Board + Ludwig to send a 'Call for Volunteers' for the roles, and
to put together the team

**AI:** Board to request release-team@opensuse.org list for this team

Discussed some of our local teams. We share concerns that those teams
with their own forums, own wikis, and own websites ultimately 'split'
the community and make it harder for everyone to benefit from the
shared knowledge, experience, and feeling of 'collective ownership' of
the project.
We'd like to see such sub-communities bought closer together and go
forward more 'aligned' with the rest of the openSUSE Project

We discussed some concerns regarding the current openSUSE Infrastructure
software.opensuse.org serves two very important roles, both as the
main download portal for our distributions, and as a software search
for OBS

**PROPOSAL:** Split software.opensuse.org to have the download portal and
search separate.

 The download portal could be a simple, clean, fast, static site that
would offer the Leap and Tumbleweed ISOs.

Software search would continue as it is...but we considered some
problems with that

  The current implementation of One-Click installs is often dangerous.
Because they add all the repos setup in the OBS repo you often end up
with crazy things like Factory:ARM repos being added on systems where
they are not relevant

  Furthermore, making it very easy to install packages from
'non-official' repos dramatically reduces the motivation and impetus
for developers to put their packages in the Distribution

  Having packages in the Distribution though is the best way to ensure
your package works, is tested, and is integrated

  So we would like to see One Click only pulling from the official repos.
  If Packages are not in the official repos, we would like the
software search to put users in touch with devel project maintainers
to encourage the packages be added to the distributions

**CALL FOR HELP:** We would like a maintainer for software.opensuse.org to
help implement the above changes to the search and download functions
of software.opensuse.org

### Meeting with the SUSE Infrastructure Team
The Board received an update from Gerhard Schlotter, Marcus 'darix'
Rueckert, and Lars Vogdt from the Infrastructure Team at SUSE
 
* SUSE host 12 physical servers for openSUSE services. This is in
addition to the 127 OBS & openQA physical servers
* Those 12 macines host a total of 60 VMs
* The OBS and openQA hardware host a total of 820 VMs
* www.opensuse.org has 2.3 million visitors per month - how can we make
that bigger?

Discussed the immediate problems with some part of the infrastructure,
especially the wiki.
Some is hosted in SUSE's datacenter in Provo, some is hosted in Nuremberg.
Nuremberg datacentre has room and admins, but limited bandwidth (not
enough for how busy stuff gets on releases).
Provo datacenter has room and bandwidth, but limited admins. SUSE have
an engineer moving from Nuremberg to Provo to help illivate that
problem.
Having sponsored hosting elsewhere is an option we want to actively
pursue. We have hardware available if we can find a host.

**CALL FOR HELP:** Please help us find sponsors willing to help find
openSUSE infrastructure

Infrastructure guys would like the Sponsorship leaflet to be updated
in order to better court possible hardware and hosting sponsors

**AI:** Douglas to update sponsorship guide

Improvements to the @opensuse.org email system are being investigated

Infra team would like connect.opensuse.org to be shutdown

**AI:** Board to investigate alternatives for voting & membership management

### Lunch
The Board had lunch with dozens of SUSE Engineers. Lots of different
conversations but the key topics that stuck with the board include:

- Discussions about how to improve translation/l10n tools and workflows
- Communication with the KDE Project
- How to get started with openSUSE, as a contributor and as a Project
that wants to be part of the openSUSE Project.

### Meeting with Ralf Flaxa - President, Product Engineering at SUSE
Ralf thanked the Board for coming and their ongoing work for the
openSUSE Project, and expressed SUSE's pleasure with the success of
Leap and the general direction of the openSUSE Project

Ralf shared some ideas regarding oSC and his departments Hackweek

**AI:** Board to discuss the ideas with the oSC organisers

### Meeting with Roland Haidl - Director, Operations & Communities at SUSE
Roland reaffirmed SUSE's intention to continue funding the openSUSE
Project at similar levels.

Roland shared Douglas DeMaio's plan to refill our merchandise before
openSUSE Conference 2016.

Board requested budget for openSUSE Asia at the same levels as last
year - **Approved**

Discussed the possibility of the Board appointing a Treasurer to be
the primary contact with SUSE on financial matters (Sponsorships, TSP,
etc) - **Approved**

Discussed the possibility of a hackathon for the Release Team, once
it's formed - **Approved** in principle (Needs the team first)

Discused the possibility of more 'minisummits' consisting of openSUSE
presentation tracks and related events colocated at other events
around the world - **Approved** in principle (Needs events and volunteers)

Discussed the current wiki problems. Roland volunteered to help drive a solution.

**AI:** Richard - Infrastructure to be a standing topic in regular
Chairman meetings with Roland

### Tour
The Board was given a tour of the SUSE HQ, including the recently
expanded office space and server rooms.
