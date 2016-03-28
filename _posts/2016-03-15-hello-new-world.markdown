---
layout: post
title:  "Hello New World!"
date:   2016-03-15 01:13:55 +0100
---
I've had to move my old blog from <http://sysrich.co.uk> to this new server on <http://rootco.de>

Most of my favourite blog posts have made the transition and have migrated from the 'old fashioned' Wordpress to the new and shiny Jekyll

It's an excuse for me to learn a bit of Ruby, practice my markdown, and keep exercising my git skills

I plan to get back to blogging more often about the goings on in my world, especially about openSUSE and openQA

And just to give Jekyll a bit of a stretch on my first real post, here's an openQA code snippit from {% include icon-github.html username="fcrozat" %}'s recent submission to
[openQA](https://github.com/os-autoinst/os-autoinst-distri-opensuse)

{% highlight perl %}
    select_console 'root-console';
    save_screenshot;

    script_run "cat /home/*/.xsession-errors* > /tmp/XSE.log";
    upload_logs "/tmp/XSE.log";
    save_screenshot;

    script_run "journalctl -b > /tmp/journal.log";
    upload_logs "/tmp/journal.log";
    save_screenshot;

    script_run "cat /var/log/X* > /tmp/Xlogs.log";
    upload_logs "/tmp/Xlogs.log";
    save_screenshot;

    script_run "ps axf > /tmp/psaxf.log";
{% endhighlight %}
