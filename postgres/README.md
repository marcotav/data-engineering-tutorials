<br>
<img align="left" width="200" src="postgres.png">

# Postgres Tutorial

## Table of contents

1. [Data Storage](#Data-Storage)
2. [Connecting to PostgreSQL](#Connecting-to-PostgreSQL)

## Data Storage
[[go back to the top]](#Table-of-contents)

This tutorial is based on [this blog article about the same topic](https://www.dataquest.io/blog/loading-data-into-postgres/).

Data storage a crucial part of any data system. It is important to understand how your data can be stored and accessed. **Data engineers** build architectures for data platforms enabling data scientists to query their data. They are responsible for building data pipelines that connect the pieces of the data ecosystem. They are familiar with:
- Working with large datasets
- Automation of intensive queries
- The architecture of robust data platforms

Each part of the pipeline below is built/maintained by a data engineer.

<br>
<img align="center" width="700" src="pipeline_mle@2x.png">

In this notebook I will describe one example **relational databases**, [`PostgreSQL`](https://www.postgresql.org/) more specifically. `PostgreSQL` is one of the main open source relational databases. It has advantages such as:
- It is easily accessible in cloud providers such as AWS
- It is highly stable
- It is open source

The `Python` library `psycopg2` one can create tables and load data into a local running `PostgreSQL` servers.










## Predicting Comments on Reddit  [[view code]](http://nbviewer.jupyter.org/github/marcotav/machine-learning-classification-projects/blob/master/predicting-number-of-comments-on-reddit-using-random-forest-classifier/notebooks/project-3-marco-tavora.ipynb) 
![image title](https://img.shields.io/badge/python-v3.6-green.svg) ![image title](https://img.shields.io/badge/ntlk-v3.2.5-yellow.svg) ![Image title](https://img.shields.io/badge/sklearn-0.19.1-orange.svg) ![Image title](https://img.shields.io/badge/BeautifulSoup-4.6.0-blue.svg) ![Image title](https://img.shields.io/badge/pandas-0.22.0-red.svg) ![Image title](https://img.shields.io/badge/numpy-1.14.2-green.svg) ![Image title](https://img.shields.io/badge/matplotlib-v2.1.2-orange.svg)

**The code is available [here](http://nbviewer.jupyter.org/github/marcotav/machine-learning-classification-projects/blob/master/predicting-number-of-comments-on-reddit-using-random-forest-classifier/notebooks/project-3-marco-tavora.ipynb) or by clicking on the [view code] link above.**


<br>
<br>
<p align="center">
  <img src="https://github.com/marcotav/predicting-the-number-of-comments-on-reddit/blob/master/Reddit-logo.png" 
       width="150" height="150">
</p>
<br>

<p align="center">
  <a href="#ps"> Problem Statement </a> •
  <a href="#steps"> Steps </a> •
  <a href="#webscraping"> Bird's-eye view of webscraping  </a> •
  <a href="#writingfunctions"> Writing functions to extract data from Reddit </a> •
  <a href="#nlp"> Quick review of NLP techniques </a> •
  <a href="#preprocess"> Preprocessing the text </a> •
  <a href="#models">Models </a> 
</p>

<a id = 'ps'></a>
## Problem Statement

Determine which characteristics of a post on Reddit contribute most to the overall interaction as measured by number of comments.

<a id = 'steps'></a>
