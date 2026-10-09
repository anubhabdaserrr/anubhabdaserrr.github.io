---
layout: page
permalink: /open-source-contributions/
title: Open-source Contributions
description: A collection of my open-source contributions, including minor fixes and improvements to existing projects. While I'm yet to make substantial contributions, I've started taking my first steps toward contributing to open-source projects.
nav: false
---

### FASTopic · June 2025

<a  href="https://github.com/bobxwu/FASTopic/"  target="_blank"  rel="noopener noreferrer">FASTopic</a> is an efficient topic modeling method, introduced in NeurIPS 2024, that uses optimal transport and pretrained Transformer embeddings to discover topics and document-topic distributions.

Contributions:
- Added a convergence monitoring feature that plots loss against epochs using `model.loss_arr` to track epoch-wise loss. [ PRs: <a  href="https://github.com/bobxwu/FASTopic/pull/13"  target="_blank"  rel="noopener noreferrer">#13</a> ]

---

### BERTopic · Dec 2022

<a  href="https://github.com/MaartenGr/BERTopic/"  target="_blank"  rel="noopener noreferrer">BERTopic</a> is a topic modeling technique that leverages transformers and c-TF-IDF to create dense clusters allowing for easily interpretable topics whilst keeping important words in the topic descriptions.

Contributions:
- Added `update_topics()` function with `diversity` and `top_n_words` parameters to customize topic representations without rerunning topic formation. [ PRs: <a  href="https://github.com/bobxwu/FASTopic/pull/887"  target="_blank"  rel="noopener noreferrer">#887</a>, <a  href="https://github.com/bobxwu/FASTopic/pull/888"  target="_blank"  rel="noopener noreferrer">#888</a> ]

---