---
layout: post
title:  "Kalium (Banano wallet) APIs &amp; Backend Rebuilt From the Ground Up"
description: "Today we are announcing the third-generation of the Kalium backend application."
date: "2022-09-02 11:10:38"
categories: ['server', 'kalium', 'apis']
score: 35
image: "https://i.imgur.com/Fjt5UHz.jpg"
tags: ['server', 'kalium', 'apis']
link: "https://banano.cc/blog/kalium-apis-backend-rebuilt-from-the-ground-up"
---

Today we are announcing the third-generation of the Kalium backend application.

## Highlights

- Kalium turned 4 years old last month.
- New backend is written in GOLang, a language that is tailored to the use case that Kalium has, that is highly concurrent and highly performant web services.
- Kalium v2.4 is a transparent upgrade for users.
- The new backend is a much more efficient, using fewer system resources by several orders of magnitude.
- It is written on GitHub, open source and MIT licensed.
- The new server is more robust, it utilizes Postgres for storing some user data such as tokens for push notifications - which solves a major pain point of the old server using Redis to store this data.

---
