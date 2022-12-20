---
layout: post
title:  "Test Driven Development from a Risk Managment Perspective"
date:   2022-12-10 10:59:30 -0500
categories: clean code
---

# Test Driven Development from a Risk Managment Perspective

Programming is not a static event. It does not occur in just one interval of time, it is a process that happens sequentially through time. Therefore we should use multiply principles instead of add principles to maximize our compounding growth. 

If we treat each programming task as a transaction between our carbon-based brains and our silicon-based brains, we can combine the best practices of the centuries-old art of trading and the craft of programming.

The goal of programming is to maximize the high quality problem we solve over time, but when solving each problem, we are faced with risks of losing mental energy, time, and money. 

If there is a cost-effective strategy could help us to minimize the risk of losing mental energy, time, and money, we should use it. Test driven development is such a strategy. It takes small losses in the short term to mitigate overall portfolio risk in the long run in a cost effective way.

The table below shows the corresponding relationship between risk management strategies and test-driven development principles:

|Risk management strategy|Example|Test-driven development principle|
|----------|----------|----------|
|Spread|Betting $5000 twice instead of $10000 at once|Refactoing test code to do the one thing|
|Diversification|Two people betting $5000 each instead of one person betting $10000|Unit tests need to be orthogonal and independent to minimize dependencies|
|Cut Losses and Stop Limit|The first rule never risk more than 2% of capital on any single trade,second if any single month the account loss more than 6%, stop trading for the rest of the moneth|Once a test fails, cut the corresponding production code ruthlessly and retreat to the previous state to rethink.
