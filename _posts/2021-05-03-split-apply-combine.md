---
layout: post
title:  "Data Manipulation in One Sentence: Split,Apply, and Combine"
date:   2021-05-03 16:45:30 -0500
categories: datascience
---

Every junior data scientist will face SQL query and basic data manipulations test.

The idea is not to confused by language syntax and case by case business needs. All data paradigm can be reduced to one sentence. Always start from the end data table your clients want.

From specific table(s), filter or apply based on multiple business needs and then recombine. 

Following are three examples,

In SQL, it's

`From X,Y SELECT, A,B WHER filter=Z GROUP BY D`

Things get interesting by replace X,Y,Z with nested SQL queries in the same format

In R, it's

`DT[i,j,by]`

In python, it's

`df.loc[x=='c',['a']].apply(lambda f:2*f)`
