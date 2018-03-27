---
layout: post
title: PIX Datacenter
header: 'PIX Datacenter: PACER Center'
subtitle: An intake tracking and reporting application built for PACER
categories: [ project ]

og_title: 'PIX Datacenter: PACER Center'
og_description: An intake tracking and reporting application built for PACER
og_image:
og_type: article
---

The Pacer Center in Bloomington MN is a non-profit organization that provides services to kids with disabilities and their parents. I became involved with The Pacer Center while employed by Ackmann & Dickenson. They were using a legacy data system that needed updating and I was a key developer of their new system called Pix Datacenter. On an intermittent basis for several years, I served as the sole developer for ongoing maintainance and new feature development.

The application itself if a fairly typical Ruby on Rails project with a simple front-end that used little more than jquery and a Postgresql database. My resposibilities were building the data models, developing data migration tools, planning deployment schedules, active bug tracking, direct client contact, and developing custom reporting tools.

Developing the data model for the Pix Datacenter project was quite challenging. It needed to track people who made contact with the Pacer Center, what their business was, and if they consumed services, what grants were involved. They needed to track this to both report back to grantors and to write applications for new grants. The better they are able to attract grant money, the more services they are able to provide. So everything needs to be woven tighly together, but in a way that accurate and useful reports can be extracted.

Once the application had been developed I wrote tools that were used to import XML data, exported from their old system, into the new PIX Datacenter application. Because the datasets were so large I had to use the (Nokogiri SAX Parser)[http://www.rubydoc.info/github/sparklemotion/nokogiri/Nokogiri/XML/SAX/Parser] to write a completely custom importer. I took a long time to run and I could have probably come up with something that would have done it faster, but this was a one-and-done process, so something slow but quick to develop was preferable.

Pacer was a close client of ours and that meant that while we did have project and client managers that would deal with them they also had direct access to me much of the time. I would handle calls directly from them if there were server issues that I had to solve. Normally more separation is preferred to keep the engineers happy, but they were a special case and I liked being in close touch with them and they did with me. It gave me a good opportunity to stretch my legs and learn to interface directly with clients even as an engineer.

The Pacer Center had a thick stack of reports they had to run monthly, quarterly, and annually. I wrote a great number of reports and eventually wrote a custom reporting system to help cut development time down for writing reports. The new system I implemented cut development time for new reports down to a quarter of what they were. This was super important for them because new requirements were always coming up the form of govermental reporting requirements or grant proposal applications.

Pacer's PIX Datacenter is one of my longest running projects, where I was a central developer in it's early development, rollout and long term mantainance. It was alo closest of all the clients I worked with at the time and one of the most rewarding to work with. It's neat to think that my software is out there helping them drive forward in their mission.
