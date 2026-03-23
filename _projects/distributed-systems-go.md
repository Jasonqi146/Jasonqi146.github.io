---
layout: page
title: Distributed Systems in Go
description: Reliable networking, RAFT consensus, and actor-model coordination built from scratch.
importance: 3
eyebrow: systems
accent: mint
stack:
  - Go
  - RAFT
  - Networking
  - Concurrency
highlight: Implemented reliable UDP transport, consensus, and actor-based state management as part of a from-scratch systems build.
---

This project was a focused exercise in building distributed systems primitives instead of only reading about them. I implemented reliable communication on top of UDP, a RAFT-based consensus system, and an actor-style runtime for coordinating multi-user state.

Most of the work lived in the failure cases: retransmission logic, leader election, state replication, and making concurrent behavior understandable enough to debug. The project sharpened my instincts around systems correctness and operational simplicity.

That perspective still carries into my current work whenever training infrastructure or evaluation environments become distributed systems problems in disguise.
