---
title: "Transactional Python for Durable Machine Learning: Vision, Challenges, and Feasibility"
collection: publications
permalink: /publication/2023-06-15-TPython
---
Supawit Chockchowaat, **Zhaoheng Li**, Yongjoo Park [(SIGMOD DEEM 2023)](http://deem-workshop.org/)

**Abstract**

In machine learning (ML), Python serves as a convenient abstraction for working with key libraries such as PyTorch, scikit-learn, and others. Unlike DBMS, however, Python applications may lose important data, such as trained models and extracted features, due to machine failures or human errors, leading to a waste of time and resources. Specifically, they lack four essential properties that could make ML more reliable and user-friendly---durability, atomicity, replicability, and time-versioning (DART).

This paper presents our vision of Transactional Python that provides DART without any code modifications to user programs or the Python kernel, by non-intrusively monitoring application states at the object level and determining a minimal amount of information sufficient to reconstruct a whole application. Our evaluation of a proof-of-concept implementation with public PyTorch and scikit-learn applications shows that DART can be offered with overheads ranging 1.5%--15.6%.
