---
layout: post
title: openSUSE Face-to-Face Board Meeting 2016 Minutes - Part 3/3
date: '2016-03-20 16:20:02 +0100'
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

This email is Part 3, containing 'big picture' strategy issues discussed

Part 1 is available [HERE]({% post_url 2016-03-20-board-meeting-f2f-2016-p1 %})

Part 2 is available [HERE]({% post_url 2016-03-20-board-meeting-f2f-2016-p2 %})

## Strategy

### Improve Visibility
Obviously, we want to improve the visibility of the openSUSE Project.

We have great distributions, great tools, and great technologies, and
we want them to be adopted by as many people and other projects as
possible.

We also want to be a natural choice for new contributors and new
projects to come to openSUSE, work with us, and host their projects
with us.

#### SUSE
SUSE is our closest, largest, partner. We have strong practical ties
with them, but that does not mean we can forget about things such as
regular clear communication and 'internal marketing'.

SUSE are working on a number of exciting new things, and it's
important that internally openSUSE is seen as a natural home for
SUSE's open source contributions.

Working closely together also should enable SUSE's corporate marketing
experts to help spread the good word about all the awesome stuff the
openSUSE Project is doing

**AI:**Bryan to investigate the possibility of Doug being invited to
Weekly team meetings for SUSE Corporate Communications

**AI:**Bryan to drive ensuring openSUSE is well integrated with SUSE's
ongoing marketing.

#### Outreach
There's no point only targeting our existing contributors and partners
like SUSE. Any open source project needs new people and with new
people comes new ideas, new solutions, and new exciting projects for
people to hack on.

A huge challenge for new contributors and projects is understanding
what is available

- Who is the openSUSE Project?
- What services do we provide?
- Where do I go to get involved?
- How do I get started?
 
These are questions which are _key_ to have simple, clear, easy to
find answers to

**CALL FOR HELP:** The Board wants to see  getting started guides for
  
 - New Users
 - New Contributors
 - New Projects- to encourage other projects to come use openSUSE as
their home

to answer the above questions. These should be simple, clear, and
relatively short. The produced guides should be easily usable on a
wiki, the website, on flyers at conferences, short blog posts..we want
to be able to spread them _everywhere_

The guides for new Contributors and new Projects are considered a
Priority by the board- to use a football related quote "There is no
point having fans, if you don't have your 11 on the pitch to play for
them"

**AI:**Board intends to create a skeleton of the above guides to help
bootstrap this idea, and will drive this, but the Board is keen to see
if anyone from the community dives in and gets to work on this
immediately.

#### Other Projects
While openSUSE is keen to see other projects call the openSUSE Project
it's home, we recognise that it's not viable for many, especially
those larger ones with their own established communities

In cases like this the Board wants to encourage strong relationships
with such Projects, and seek out partnerships and other arrangements
with such Projects for the benefit of all involved

Examples include ownCloud and Kolab, where we believe openSUSE is in a
perfect position to offer tools, community, and a solid environment
for these projects to use as a default or recommended platform for
their users

**AI:**Bryan to arrange information exploratory discussions

#### Hardware vendors
Having hardware sponsors and partners is nice but is hard. Solid
hardware support requires the hardware to be available and in the
hands of the right contributors to make it happen.

Otherwise there is no way how to support special hardware without the
things available for testing.

However, we do have some relationships which are happening, and we
want to highlight those who do stuff with us, such as

- Soft Iron are shipping 64-bit ARM servers with openSUSE Tumbleweed as standard
- Fujitsu offer openSUSE Tumbleweed to thier customers who want a
Linux option on their Desktop & Server Hardware
- Epson have some printers using openSUSE and YaST
- Open Mainframe are investigating the possibility of building an
openSUSE distribution for s390x

## Reform and Remove Mess
Improving viability and reaching out to new areas is all well and
good, but we need to make sure the project internals are tidy, clear,
and easy to use

The Board discussed the state of many infrastructure and project policies
and processes.

We agreed a principle of, when something is imperfect, we Reform (aka
improve) or Remove it.

Services identified to be removed or reformed:

- Software.o.o:
  - Media download needs to be easier, prefferable static page
  - package search adds too much mess to the installed systems.
Invalid repos should not be distributed by 1-click installs
  - somehow redesign and reduce confusion to ensure that users
do not end up with 80+ additional repos.
- Wiki:
  - In order to fix the wiki quickly ,the board approved the
idea of deploying the latest version of mediawiki on a new server
without branding
  - branding can always be redone later
- Blogs/Planet:
  - Only a handful of people use lizards, but it takes a lot of
resources to keep it running. We want to shut it down, and encourage
it's users move to their own blogs, which will then be aggregated on
planet.opensuse.org
  - Improve planet.opensuse.org. Find a maintainer, use a clean
upstream OSS soltion if possible
 
**AI:**Kostas to contact the few Lizards bloggers to discuss
their migration options

- News.o.o:
  - Wordpress consumes too many resources and poses too many
security risks
  - Replace with something lightweight
 
**AI:**Richard talk with Douglas about this

- i18n.o.o: Translations site is being migrated to l10n.o.o as we speak
and i18n will be killed including the svn prior Leap 42.2 release.
- Legal layout of Board/membership:
 The current layout of the Board Election Rules, Membership
Rules, and such are sometimes confusing and missing some details
 The documents will be updated and restructured to be more clear
 This should set the framework for discussing any reforms of
the Membership process once the Membership tidy-up is complete

**AI:**board- get Infra team to provide list of services we have, soon
to help with this endevour
