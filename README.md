---
title: SENG 550 Project Proposal
author: Stéphane Dorotich
date: Dec 15th, 2022
documentclass: scrartcl
---

> Repository: [https://github.com/stephanedorotich/550](https://github.com/stephanedorotich/550).
>
> I attest that all work is my own and that I worked on this project by myself. Stéphane Dorotich, UCID: 10154487

# Abstract

Needs:
- Description of proj + main outcomes

# Introduction

:::columns

Language is fluid, nuanced, and diverse. Our voices are like fingerprints. We express ourselves according to our interests, knowledge, education, culture, and environment. The way we speak is a reflection of our experiences.

To presume that language emerges from a finite set of words is naive. Yet mathematicians are want to believe it is so. But such an unflavorful perspective denies all the richness that our voices truly carry.

The complexity of language is an algorithmic behemoth. It eludes even the finest of minds. But language is the backbone of communication. Understanding it's fabric is a great endeavor. So here we stand, with primitive tools such as Linear Regression and Neural Networks attempting to chisel the masterpiece of language from text corpora. Perhaps, as Michelangelo did, we can achieve some of the beauty of reality. To me, however, it feels like carving a masterpiece with wooden tools.

But here I am, with wooden tools. At present, I neither have the knowledge nor the skill to create a masterpiece. What I can do, however, is learn how to use my tools.

## Problem

Sentiment analysis is a crude beginning for language comprehension. I say this because language comprehension transcends simple binary classification problems; but - as with everything - you must begin somewhere. For this project, I begin with a simple binary classification problem of determining if Amazon Reviews are positive, or negative.

## Background and Related Work

Sentiment Analysis has been a burgeoning field of research for nearly 20 years. More than 99% of papers on the topic have been published since 2004 [@mm2017]. Since large corpora of text became widely available on the internet (and in emergence of Big Data) it has become both an exciting area of research as well as a desireable commercial enterprise.

There are three established approaches to Sentiment Analysis [@mw2022] a Lexicon Based Approach, a Machine Learning Approach, and a Hybrid Approach.

The Lexicon based approach begins with a dictionary. This dictionary assigns a score to each token (word) in a document that is positive or negative depending on how strongly it correlates to the outlook of the document, usually the value is in the range [-1, 1] where the extreme ends indicate extreme negative or positive association. A document (review) is parsed word by word and a cumulative total is computed using the scores from the Lexicon. A negative score indicates negative sentiment while a positive score indicates a positive sentiment. This approach has limited applications because of the domain specific knowledge required to develop the lexicon, as Wankhade [@mw2022] put it - "given the word 'small' and the sentences 'The TV screen is too small' and 'This camera is extremely small', the word 'small' in the first sentence is negative, as people generally prefer large screens, whereas in the second sentence it is positive, as if the camera is small, it will be easy to carry".

I appreciate that the Lexicon approach considers the context in which the reviews are being made, however, this strength is also it's greatest weakness. The Lexicon Based approach is not generalizeable. In order to move the model to a new domain, the lexicon must be redeveloped - this is neither scallable nor time efficient.

Although the hybrid approach is intriguing, it is beyond the scope of this project.

Instead, I will focus on the Machine Learning approach, specifically using a Regularized Logistic Regression model to develop a binary classifier. This approach will be described in more detail later.

## Applications

In the context of Amazon reviews, determining whether a review is positive or negative is neither interesting nor useful. Amazon reviews have *ratings* making sentiment evident. However, developing a generalized sentiment classifier can be useful if it can be taken into new contexts. For instance, a general sentiment analysis method could be used on Tweets or on YouTube comments to determine how a population feels about a particular news event, company, or idea.

## Goals

Foremost, my goal is to explore Natural Language Processing (NLP). I have been curious about NLP for a long time, but have not had any opportunities to explore it (save for taking a handful of Linguistics courses.) My goal is not to develop the next greatest Sentiment Analysis model, there are already models that far exceed anything I could develop on my own.

My goal, instead, is to demonstrate that using NGrams as features for a Regularized Logistic Regression model is more accurate than using just 1-Grams (single words) as features for a Regularized Logistic Regression model. My hypothesis is that because NGrams help carry contextual information alongside words, it helps weed through some of the nuances of language. For example, the 3-gram "not very good" obviously carries a negative sentiment. Whereas when considered as 1-grams "not", "very", "good" it is difficult to distinguish from the positive review "Not a day goes by that I don't use it. Very good!" which contains the same 1-grams.

My hypothesis is that any method that improves the contextual awareness of a Machine Learning algorithm will improve it's precision. I will not be able to prove this hypothesis, but I do hope to support it.

## Data Analysis Question

Does a 1-Gram mixed with a 2-Gram Bag-of-Words Regularized Logistic Regression model have greater **precision** than a similar 1-Gram model?

How do their **accuracy** and **recall** compare?

:::

# Background and related work

Needs:
- Technical background help for understanding report (if relevant)
    1. Sentiment Analysis
    2. Bag-of-Words
    3. Tf-Idf
    4. NGrams
    5. Bag-of-NGrams
- Review of existing work pertinent to your project
    hmmm....

Blah blah [@mw2022]

# Methodology

Needs:
- Experiment setup
- Experimentation factors (types of ML algorithms, hyperparameters tuned, details on training/test/cross-validation data set)
- Experiment process
- Performance metrics - accuracy, precision, recall, F-score, etc. ?

# Results

Needs:
- Key findings in your exploratory data analysis and prediction. Compare results?
- Conclusions & future work
    - Multiclass Logistic Regression




M. Wankhade, A. C. Rao, and C. Kulkarni, “A survey on sentiment analysis methods, applications, and challenges,” Artificial Intelligence Review, vol. 55, no. 7, pp. 5731–5780, 2022. 


IEEE double column conference format

# Reference