---
title: Telegram Analysis
category: NGO Social Media Analysis
menu_order: 3
order: 2
---

Firstly, 10 topics LDA for telegram channels and chats was created to explore the data:

{% include lda_layout.html width="830" height="700" src="https://raw.githubusercontent.com/Teplitsa/CSRLab/main/docs/_includes/LDAModel_cleanstops.html" %}

Then coherence was calculated for LDA models from 4 to 20 topics in order to define the optimal number of topics. According to the graph below 4 topics are the best fit:

{% include coherence_lda.html %}

However, LDA for 4 topics seems to have less topics then there actually are in the data. For instance, in 10-topics LDA model there is a topic about kids\health\schools\help. While 4 topics data seems to talk only about news and human rights activism. Clearly NGOs in our dataset are much more diverse than that.

{% include lda_layout.html width="830" height="700" src="/NGO_Social_Media_Analysis/LDAModel_cleanstops_4top.html" %}
