---
title: "REFORM: Fast and Adaptive Solution for Subteam Replacement"
collection: publications
permalink: /publication/2020-11-15-REFORM
---
Zhaoheng Li, Xinyu Pi, Mingyuan Wu, Hanghang Tong (In submission)

**Abstract**

In this paper, we propose the novel problem of Subteam Replacement: given a team of people embedded in a social network to complete a certain task, and a subset of members – subteam - in this team which have become unavailable, find another set of people who can perform the subteam’s role in the larger team. The ability to simultaneously replace multiple team members is highly appreciated in settings such as corporate management where team structure is highly volatile and large-scale changes are commonplace. We conjecture that a good candidate subteam should have high skill and structural similarity with the replaced subteam while sharing a similar connection with the larger team as a whole. Based on this conjecture, we propose a novel graph kernel which evaluates the goodness of candidate subteams in this holistic way freely adjustable to the need of the situation. To tackle the significant computational difficulties, we combine our kernel with a fast approximate algorithm which (a) employs effective pruning strategies, (b) exploits the similarity between candidate team structures to reduce kernel computations, and (c) features a solid theoretical bound obtained from mathematical properties of the problem. We extensively test our solution on both synthetic and real datasets to demonstrate its consistency and efficiency. Our proposed graph kernel results in more suitable replacements being proposed compared to graph kernels used in previous work, and our algorithm consistently outperforms alternative choices by finding near-optimal solutions while scaling linearly with the size of the replaced subteam.
