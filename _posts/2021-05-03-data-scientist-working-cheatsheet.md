---
layout: post
title:  "Data Scientists' Working Cheatsheet(ongoing)"
date:   2024-08-28 16:45:30 -0500
categories: datascience
lang: en
---
## A Data Scientists' Core metrics

M = How fast you can build a workable solution X How fast your machine can run your soltion X How much and how large positive impact your solution can make 

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

## How to manipulate your dataframe fast?
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

#### STYLES OF DOCUMENTATION

1. One topic at a paragraph. 
2. Begin with topic sentence and follow with a specific example. Don’t forget examples.
3. Use positive and active tones. 
Negative: He is not often on time.
Positive: He usually comes late.

### Junior vs Senior Data Scientist

|                 | Junior                                                       | Senior                                                       |
| --------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Ambition        | 1. Make no mistakes and make everything look good and compliant to best practice | 1. Build something new                                       |
| Process         | 1. Start to end is very random                               | 1. Among massive random trials, hide a structured bidirectional BFS+shortest search from end to start |
| Stage           | 1. All energy spent on modeling                              | 1. More energy spent on shipping and iterating               |
| Communication   | 1. Explain how sometimes with jargon                         | 1. Explain why, impact, cost in plain English                |
| Problem Scoping | 1. Greedy                                                    | 1. Start very small, one feature at a time                   |
| Evaluation      | 1. Only use one or two metrics<br/>2. Sometimes use vanity metrics and ignore counter-metrics | 1. Consider both explicit and implicit metrics, will use counter-metrics and proxy metrics if necessary<br>2. Set metrics in advance not after the fact |
| Data            | 1. Never consider about sampling bias <br/>2. Lack the ability to scrape and handle unstructured data <br/>3. A lot of for loop or apply lambda function in pandas operations | 1. Am I introducing the bias when sampling <br/>2. Feel comfortable to use API to handle unstructured data<br/>3. Bit masking, vectorization in matrix operation, use matrix decomposition and multiplication to fasten the if else logic |
| Model           | 1. Follow the hottest trend                                  | 1. Start a simple model to get whole pipeline running<br>2. Leverage on the current working soluion |
| Deployment      | 1. Hardly think about it                                     | 1. Think about deployment from day one                       |
| Working Memory  | 1. Listen to the music, phone is next to your working table and open 20 windows at the same time<br/>2. Switch context very often | 1. Be very aware of working memory boundaries, phones shut down, at most three windows, use plain text as much as possible<br/>2. One block of code at a time |
| Decision Making | 1. Decide based on probability                               | 1. Decide based on payoff, there's no such thing as data scientist 20 years ago, but there's trader, investor, hedger, and arbitarger 2 centuries ago. |
| Problem Solving | 1. Trial and error                                           | 1. Know multiple heuristics(How to solve it?)                |
| Reasoning       | 1. Inductive reasoning a lot<br>2. Have only one hypothesis in head | 1. Use all deductive, inductive, and abductive reasoning<br>2. Have at least two or even multiple competing hypothesis in head at the same time |

