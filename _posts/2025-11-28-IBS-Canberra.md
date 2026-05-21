---
title: "IBS Canberra: Bayesian Ordinal Regression for Crop Development and Disease Assessment"
date: 2025-11-28
categories: [Conference, Statistics, Research]
tags: [IBS, Canberra, Presentation, Bayesian Methods, Ordinal Regression, Crop Development, Disease Assessment]
---

I presented at the International Biometric Society (IBS) meeting in Canberra (November 2025), sharing recent developments in Bayesian ordinal regression methods for analysing crop development and disease severity data from field trials.

## 📋 Abstract

Accurate assessment of crop development and disease severity is essential for informed agronomic decision-making. This study presents a **Bayesian framework for analysing ordinal data** from field trials, including growth scale progression and disease ranking scores. Using the **brms package in R**, we applied cumulative logit models to evaluate the effects of sowing depth and treatment combinations on cereal growth stages, measured via the **Zadok's scale**, across two Western Australian sites (Merredin and Wickepin). The same framework is being extended to model disease severity scores, demonstrating its versatility across categorical biological measurements.

Our workflow incorporates rigorous model testing and evaluation, including **posterior predictive checks** and **leave-one-out cross-validation (LOO-CV)**, to ensure robust inference and model fit. Rather than relying on p-values from linear mixed models, the Bayesian approach provides **interpretable probabilities** of achieving specific growth stages or disease severity levels. This shift enables more nuanced understanding of treatment effects and supports decision-making under uncertainty.

## Authors
**Zhanglong Cao**, Rose Megirian, Matthew Nguyen, Adam Sparks

### Downloads
- 🌐 [Interactive HTML Presentation]({{ site.baseurl }}/assets/quarto/2025-11-28-IBS.html)

## 🎯 Key Topics Covered

- **Ordinal regression** using Bayesian methods (brms package)
- **Cumulative logit models** for growth stages and disease severity
- **Zadok's scale** and categorical biological measurements
- **Model validation**: Posterior predictive checks and LOO-CV
- **Field trials**: Multi-site comparisons (Merredin, Wickepin)
- **Treatment effects** on cereal development and disease ranking
- **Decision-making under uncertainty** using posterior probabilities

## 💡 Highlights

The key innovation was moving beyond traditional p-value inference to Bayesian posterior probabilities, which directly answer practically important questions: *"What is the probability this treatment advances growth stages?"* or *"What is the likely disease severity range given these conditions?"* This probabilistic framework is particularly well-suited to ordinal data from field trials, where nuance in ranking and progression matters more than binary significance testing.

The multi-site evaluation (Merredin and Wickepin) demonstrated robustness of the Bayesian ordinal regression approach across diverse Western Australian growing environments, and the extensibility to disease severity scores opens pathways for integrated crop health modelling.

## 🙏 Acknowledgments

Thank you to the International Biometric Society and the Canberra organising committee for the invitation and the opportunity to share this work with the biometric and agricultural statistics community. Special thanks to all attendees for their thoughtful questions and constructive feedback.
