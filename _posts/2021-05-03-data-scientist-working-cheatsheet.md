---
layout: post
title:  "Data Scientists' Working Cheatsheet"
date:   2021-05-03 16:45:30 -0500
categories: datascience
---

## How to communicate and sell your model?

To get buy in and sell your model to different stakeholders is hard.

Whatever your pitch is, include these seven talking points will definitely help:

1. What's the problem you are trying to solve?
2. Why you think it's a problem worth solving?
3. How machine learning, deep learning or data science can help?
4. How will this data product consumed by customers?
5. Where will this data product fit into product or business lines?
6. Here's a visualization of proposing data product?
7. Ask questions, critics, feedbacks and concerns from audience.


## Data Manipulation in One Sentence: Split,Apply, and Combine

Every junior data scientist will face SQL query and basic data manipulations test.

The idea is not to be confused by language syntax and case by case business needs. All data paradigm can be reduced to one sentence. Always start from the end data table your clients want.

From specific table(s), filter or apply based on multiple business needs and then recombine. 

Following are three examples,

In SQL, it's

`From X,Y SELECT, A,B WHER filter=Z GROUP BY D`

Things get interesting by replace X,Y,Z with nested SQL queries in the same format

In R, it's

`DT[i,j,by]`

In python, it's

`df.loc[x=='c',['a']].apply(lambda f:2*f)`

## How to document and save yourself?

To document well is to save your future self. One minute spent in good documentation

saves you hours or work in debugging, recalling and guessing your past self.

### Five Topics of Documentation

1. Use one sentence to describe what problems you are trying to solve.

2. What algorithms you use to solve that problem.

3. How you implement that algorithm.

4. What blocks and major challenges you’ve conquered?

5. Where can find related references, notes and tools?

### STYLES OF DOCUMENTATION
1. One topic at a paragraph. 

2. Begin with topic sentence and follow with a specific example. Don’t forget examples.

3. Use positive and active tones. 

Negative: He is not often on time.

Positive: He usually comes late.
