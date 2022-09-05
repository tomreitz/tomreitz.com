---
title:  "Logservatory"
permalink: "/posts/logservatory"
categories: ["data", "processing"]
header:
  teaser: /assets/images/projects/logservatory.jpg
excerpt: >
  A Python and SQLite tool for querying website access logs.
---

In spring 2021, I did a project for my *foundations of data management* class where I built a Python and SQLite tool for processing website access logs. The tool is fairly efficient because it reads log files from disk only once but can run any number of queries over them. Moreover, it can process streaming logs in realtime, which can make it a useful tool for detecting and blocking credential stuffing, scraping, and other attacks.

<center>
<a class="btn btn--info btn--primary" href="https://github.com/tomreitz/logservatory" target="_blank">Code</a>
<br />
</center>

Using logservatory, I analyzed the website access logs of Ballotpedia.org (my employer at the time) for the entire year 2020 &mdash; 3.2 billion requests, 1.4 TB of log files (uncompressed). Results of the analysis can be found in the video presentation below.

{% include video id="XXQoKTHLAW" provider="youtube" %}
