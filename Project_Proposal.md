---
title: SENG 550 Project Proposal
author: Stéphane Dorotich
date: Nov 26th, 2022
---

# Project Description

In this project, I will develop a Sentiment Analysis ML model that predicts Positive, Neutral, and Negative sentiment based on the text of Amazon reviews.

## Application

Because most reviews are paired with a star-rating, the application of this model is fairly limited (since the star-rating can be used as a direct measurement of sentiment.) It may, however, have applications in Tweet Sentiment analysis. For example, to discover the sentiment of Tweets about a particular company.

## Goal

My goal is to learn about Natural Language Processing, it has long been an interest area of mine.

## Data Source

Jianmo Ni, Jiacheng Li, and Julian McAuley. 2018. Amazon Review Data \[json\]. Retrieved from [https://nijianmo.github.io/amazon/index.html](https://nijianmo.github.io/amazon/index.html)

## Objectives

| Number | Description |
|:------:|:------------|
| 1 | Create datasets for Training/Validation/Testing |
| 2 | Use Spark to create n-gram models for each document
| 3 | Use Spark to create a feature list for documents that uses the tf-idf of each n-gram |
| 4 | Develop a ML model to predict sentiment |