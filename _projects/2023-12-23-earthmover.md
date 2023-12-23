---
title:  "earthmover"
permalink: "/posts/earthmover"
categories: ["data", "transformation"]
header:
  teaser: /assets/images/projects/earthmover.png
excerpt: >
  A CLI tool for transforming collections of tabular source data into a variety of text-based data formats via YAML configuration and Jinja templates.
date: 2023-12-23

---

![earthmover](../assets/images/projects/earthmover.png)

[earthmover](https://github.com/edanalytics/earthmover) is a command-line data transformation tool I've built as part of my work at [Education Analytics](https://www.edanalytics.org/). It
 * loads data from a variety of sources, including CSV and other types of files, relational database connections, and more
 * transforms the data according to instructions in a YAML file
 * renders a [Jinja](https://jinja.palletsprojects.com/en/3.1.x/) template (which can be any text-based data format, including JSON, XML, HTML, YAML, and more) for each row of transformed data, and saves the output to a file

`earthmover` is similar in some ways to [dbt](https://www.getdbt.com/), but it *is* the transformation execution engine (rather than issuing SQL commands to a database backend which is the execution engine). `earthmover` is built using a number of Python libraries including [Dask](https://www.dask.org/) and [NetworkX](https://networkx.org/).

At EA, we use `earthmover` to transform various types of flat files into JSON according to the [Ed-Fi](https://www.ed-fi.org/) data standard, which we then send to Ed-Fi APIs using [lightbeam](/posts/lightbeam). You can learn more about both tools in [this presentation](https://tomreitz.github.io/edfi-earthmover-lightbeam-slides/).
