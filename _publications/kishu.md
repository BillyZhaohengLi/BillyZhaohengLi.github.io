---
title: "Kishu: Time-Traveling for Computational Notebooks"
collection: publications
permalink: /publication/2024-10-15-Kishu
---
**Zhaoheng Li**, Supawit Chockchowwat, Ribhav Sahu, Areet Sheth, Yongjoo Park [(VLDB 2025)](https://vldb.org/2025/)

**Abstract**

Computational notebooks (e.g., Jupyter, Google Colab) are widely used by data scientists. A key feature of notebooks is the interactive computing model of iteratively executing cells (i.e., a set of statements) and observing the result (e.g., model or plot). Unfortunately, existing notebook systems do not offer time-traveling to past states: when the user executes a cell, the notebook session state consisting of user-defined variables can be irreversibly modified—e.g., the user cannot ’un-drop’ a dataframe column. This is because, unlike DBMS, existing notebook systems do not keep track of the session state. Existing techniques for checkpointing and restoring session states, such as OS-level memory snapshot or application-level session dump, are insufficient: checkpointing can incur prohibitive storage costs and may fail, while restoration can only be inefficiently performed from scratch by fully loading checkpoint files. In this paper, we introduce a new notebook system, Kishu, that offers time-traveling to and from arbitrary notebook states using an efficient and fault-tolerant incremental checkpoint and checkout mechanism. Kishu creates incremental checkpoints that are small and correctly preserve complex inter-variable dependencies at a novel Co-variable granularity. Then, to return to a previous state, Kishu accurately identifies the state difference between the current and target states to perform incremental checkout at sub-second latency with minimal data loading. Kishu is compatible with 146 object classes from popular data science libraries (e.g., Ray, Spark, PyTorch), and reduces checkpoint size and checkout time by up to 4.55× and 9.02×, respectively, on a variety of notebooks.
