---
title:  "lightbeam"
permalink: "/posts/lightbeam"
categories: ["data", "movement"]
header:
  teaser: /assets/images/projects/lightbeam.png
excerpt: >
  A CLI tool for validating and transmitting payloads from JSONL files into an Ed-Fi API.

---

![lightbeam](../assets/images/projects/lightbeam.png)

[lightbeam](https://github.com/edanalytics/lightbeam) is a command-line tool for interacting with [Ed-Fi](https://www.ed-fi.org/) APIs, which I've built as part of my work at [Education Analytics](https://www.edanalytics.org/). It can
 * `count` records in an Ed-Fi API
 * `fetch` JSON payloads from an Ed-Fi API
 * `validate` JSON payloads against the Swagger of an Ed-Fi API
 * `send` JSON payloads to an Ed-Fi API
 * keep track of state, to avoid resending payloads that have already been transmitted

`lightbeam` makes asynchronous HTTP requests to achieve remarkable performance of 100 requests per second or more.

At EA, we use [earthmover](https://github.com/edanalytics/earthmover) to transform various types of flat files into JSON according to the [Ed-Fi](https://www.ed-fi.org/) data standard, which we then send to Ed-Fi APIs using `lightbeam`. You can learn more about both tools in [this presentation](https://tomreitz.github.io/edfi-earthmover-lightbeam-slides/).
