---
layout: post
title: Watchmen AR
header: Watchmen AR
subtitle: Remote monitoring and notification with barebones Rails server
categories: [ project ]
tags: [ 'Web Development', 'Ruby on Rails', PostgreSQL, Bootstrap, HTML, CSS, Heroku ]

og_title: Watchmen AR
og_description: Remote monitoring and notification with barebones Rails server
og_image: /assets/images/watchmen-ar.jpg
og_type: article
---

![bus stop]({{site.url}}/assets/images/watchmen-ar.jpg)

Watchmen AR was an augmented reality project, developed by [Puzzlefox Interactive](http://puzzlefox.co/), that I lent a helping hand to in 2019. My part in it was connecting remote Unity apps, deployed to NY and LA, with the developers here in MN.

The requirements were pretty simple. First, they needed a way for remote Unity apps to retrieve a configuration file. Second, they needed to be able to log data about running status of the machines on a regular basis. And finally, they needed emails to be sent if the machines failed to perform the AR experience.

All of this was solved with a barebones 'Rails server, deployed to Heroku. The server exposed a few API endpoints for retrieving the configuration file and for logging. Admins could log in, adjust configurations for each of the deployed apps and browse log files. There were also API endpoints exposed for the apps to check in. The server ran a job (Heroku Scheduler) that checked if the apps had checked in recently--if not it sent off an email to the admins to notify them.

This was a super simple build, but filled a crucial gap in the project. It was a perfect demonstration of the power of custom one-off software development.


