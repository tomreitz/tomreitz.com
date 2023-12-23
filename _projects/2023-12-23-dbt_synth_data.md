---
title:  "dbt_synth_data"
permalink: "/posts/dbt_synth_data"
categories: ["data", "synthetic"]
header:
  teaser: /assets/images/projects/dbt_synth_data.png
excerpt: >
  A dbt package for creating synthetic data on several backends.
date: 2023-12-23

---

![dbt_synth_data](../assets/images/projects/dbt_synth_data.png)

[dbt_synth_data](https://github.com/edanalytics/dbt_synth_data) is a [dbt package](https://docs.getdbt.com/docs/build/packages) I've built as part of my work at [Education Analytics](https://www.edanalytics.org/). The package's features include:
* support for [Snowflake](https://www.snowflake.com/en/), [Postgres](https://www.postgresql.org/), [SQLite](https://www.sqlite.org/index.html), and [DuckDB](https://duckdb.org/) backends
* ability to generate various distributions including normal, exponential, binomial, and more
* ability to combine basic distributions by union or average to create more complex ones
* ability to generate many basic data types including boolean, numeric, string, and date
* ability to generate more complex data types including references to other tables, words, names, and addresses
* impressive performance, with ability (on Snowflake) to create billions of rows and hundreds of GB of synthetic data

At EA, we use [dbt_synth_data](https://github.com/edanalytics/dbt_synth_data) to create synthetic data in the [Ed-Fi](https://www.ed-fi.org/) data standard, which can then be used for
* testing user interfaces
* demoing applications to users without permission to access real data
* performance-tuning operational systems
* preparing training and other materials with realistic data

You can learn more about `dbt_synth_data` in [this presentation](https://tomreitz.github.io/dbt_synth_data_slides/).
