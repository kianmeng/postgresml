---
author: Montana Low
description: A common problem with data science and machine learning tutorials is the published and studied datasets are often nothing like what you’ll find in industry.
image: https://postgresml.org/images/illustrations/uml.png
image_alt: Data is relational and growing in multiple dimensions
---


<style>
img.float-right {
  margin: 0 16px !important;
  max-width: 50%  !important;
  float: right;
}
img.float-left {
  margin: 0 16px !important;
  max-width: 60%  !important;
  float: left;
}
img.center {
  margin: 16px 12.5%;
  max-width: 75%;
}
</style>

Data is Living and Relational
================================

<p class="author">
  <img width="54px" height="54px" src="/images/team/montana.jpg" />
  Montana Low<br/>
  August 25, 2022
</p>


A common problem with data science and machine learning tutorials is the published and studied datasets are often nothing like what you’ll find in industry.

<center markdown>

  | width | height | area  |
  | ----- | ------ | ----- |
  | 1 | 1 | 1 |
  | 2 | 1 | 2 |
  | 2 | 2 | 4 |

</center>

They are:

- usually denormalized into a single tabular form, e.g. a CSV file
- often relatively tiny to medium amounts of data, not big data
- always static, with new rows never added
- sometimes pretreated to clean or simplify the data

As Data Science transitions from academia into industry, these norms influence organizations and applications. Professional Data Scientists need teams of Data Engineers to move data from production databases into data warehouses and denormalized schemas, which are more familiar and ideally easier to work with. Large offline batch jobs are a typical integration point between Data Scientists and their Engineering counterparts, who primarily deal with online systems. As the systems grow more complex, additional specialized Machine Learning Engineers are required to optimize performance and scalability bottlenecks between databases, warehouses, models and applications.

This eventually leads to expensive maintenance and terminal complexity: new improvements to the system become exponentially more difficult. Ultimately, previously working models start getting replaced by simpler solutions, so the business can continue to iterate. This is not a new phenomenon, see the fate of the Netflix Prize.

Announcing the PostgresML Gym 🎉
-------------------------------

Instead of starting from the academic perspective that data is dead, PostgresML embraces the living and dynamic nature of data produced by modern organizations. It's relational and growing in multiple dimensions.

![relational data](/images/illustrations/uml.png)

Relational data:

- is normalized for real time performance and correctness considerations
- has new rows added and updated constantly, which form incomplete features for a prediction

Meanwhile, denormalized datasets:

- may grow to billions of rows, where single updates multiply into mass rewrites
- often span multiple iterations of the schema, with software bugs leaving behind outliers

We think it’s worth attempting to move the machine learning process and modern data architectures beyond the status quo. To that end, we’re building the PostgresML Gym, a free offering, to provide a test bed for real world ML experimentation, in a Postgres database. Your personal Gym will include the PostgresML dashboard, several tutorial notebooks to get you started, and access to your own personal PostgreSQL database, supercharged with our machine learning extension.

<center>
  <video controls autoplay loop muted width="90%" style="box-shadow: 0 0 8px #000;">
    <source src="https://static.postgresml.org/postgresml-org-static/gym_demo.webm" type="video/webm">
    <source src="https://static.postgresml.org/postgresml-org-static/gym_demo.mp4" type="video/mp4">
    <img src="/images/demos/gym_demo.png" alt="PostgresML in practice" loading="lazy">
  </video>
</center>

<center markdown>
  [Try the PostgresML Gym](https://cloud.postgresml.org/){ .md-button .md-button--primary }
</center>

Many thanks and ❤️ to all those who are supporting this endeavor. We’d love to hear feedback from the broader ML and Engineering community about applications and other real world scenarios to help prioritize our work. 
