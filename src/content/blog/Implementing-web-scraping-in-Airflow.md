---
author: Julius
pubDatetime: 2024-03-19T20:14:39.000Z
modDatetime: 
title: Implementing web scraping in Airflow
featured: false
draft: true
tags:
  - web
  - data
  - automation
description: A new exploration of using Airflow to schedule and manage web scraping
---

Airflow can be used with many tasks. I'm sure web scraping are very common before.

Searching for web for a while, no clear article about how to use headless browser with airflow. While it is not ideal for large scale web scraping (you would need javascript reverse engineering for most of the sites), it is still more suitable for small size data scraping, arguably could be empowered by Airflow.