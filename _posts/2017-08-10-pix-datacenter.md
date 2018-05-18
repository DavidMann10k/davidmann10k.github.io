---
layout: post
title: PIX Datacenter
header: 'PIX Datacenter: PACER Center'
subtitle: An intake tracking and reporting application built for PACER
categories: [ project ]
tags: [Ruby on Rails, 'Web Development', PostgreSQL, Ruby, HTML, CSS, SASS, JavaScript, jQuery, Rackspace, Ubuntu]

og_title: 'PIX Datacenter: PACER Center'
og_description: An intake tracking and reporting application built for PACER
og_type: article
---

The Pacer Center in Bloomington Minnesota is a non-profit organization that provides services to kids with disabilities and their parents. I became involved with The Pacer Center while employed by Ackmann & Dickenson. They were using a legacy data system that needed updating, and I was a key developer of their new system called Pix Datacenter. On an intermittent basis for several years, I served as the sole developer for ongoing maintenance and new feature development.

The application itself is a Ruby on Rails project with a simple front-end that used a jQuery and a Postgresql database. My responsibilities were building the data models, developing data migration tools, planning deployment schedules, tracking active bugs, acting as the direct client contact, and developing custom reporting tools.

Developing the data model for the Pix Datacenter project was quite challenging. It needed to track people who made contact with the Pacer Center, what their business was, and, if they consumed services, what grants were involved. Pacer needed to track this to both report back to grantors and to write applications for new grants. The better they are able to attract grant money, the more services they are able to provide. So everything needs to be woven tightly together, but in a way that is accurate and useful reports can be extracted.

Once the application had been developed, I wrote tools that were used to import XML data, exported from their old system, into the new PIX Datacenter application. Because the data sets were so large I had to use the Nokogiri SAX XML Parser to write a specialized importer. Because this was a one time data conversion, it was more important to have the tool developed quickly than to have it process all the data quickly. In the end, the import tool was slow, but it accurately converted the data needed within the budget and development schedule constraints.

Although the project was managed by project and client managers, the client also had direct access to me. I would handle calls directly from my client partners if there were server issues. I also worked with them directly to understand application issues and enhancement requirements. I liked being in close touch with them, and they did with me. It gave me a good opportunity to stretch my legs and learn to interface directly with clients even as an engineer.

The Pacer Center had a thick stack of reports they had to run monthly, quarterly, and annually. I wrote over 30 custom reports and eventually architected a reporting system to help cut development time down for writing reports. The new system I implemented cut development time for new reports down to a quarter of what it was originally. Quick turnaround for new report development was important because governmental reporting, and new grant proposal applications requirements were continually changing.

Pacer's PIX Datacenter is one of my longest running projects, where I was a central developer in its early development, rollout and long term maintenance. I worked more closely with them than any other clients. It was rewarding to develop and maintain an application that is integral to the Pacer Center's ability to drive forward in their mission.
