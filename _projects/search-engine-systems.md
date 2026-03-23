---
layout: page
title: Search Engine Systems
description: A Java and Lucene retrieval stack covering BM25, Indri, learning-to-rank, and diversification.
importance: 4
eyebrow: information retrieval
accent: ink
stack:
  - Java
  - Lucene
  - BM25
  - Learning to rank
highlight: Built a search stack that moved from classical IR baselines to ranking and diversification in one cohesive system.
---

I built this project as an end-to-end search engine library in Java with Lucene as the indexing backbone. The goal was to cover the full retrieval pipeline instead of treating ranking methods as isolated homework exercises.

The system implemented BM25, Indri-style retrieval, learning-to-rank, and diversification, with enough structure to compare retrieval strategies cleanly. It was a good forcing function for thinking about interfaces, evaluation, and the relationship between ranking quality and system design.

That foundation has been surprisingly durable: a lot of modern LLM evaluation and retrieval work still reduces to careful information access and ranking choices.
