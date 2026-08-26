---
layout: default
title: Model Evaluation
---

## Оглавление
* TOC
{:toc}

# Metrics

# Train / validation / test

# Настройки
## Логирование

# Rules of Machine Learning

# Leakage

# Temporal evaluation
Классическая задача - по прошлому предсказывать будущее. Как это делать? Самый простой и достаточно популярный способ - time split. Однако, если задуматься, то это ведь очень сильный claim. Допустим, мы делим данные в отношении 8:1:1 (train, valid, test): по первым 80% предсказать следующие 20%. Где гарантия, что здесь нет утечки?

Рассмотрим такой пример: пользователь покупает товары, первые 80% это только белые кроссовки в определенном стиле, сдедующие 10% тоже кроссовки, следующие 10% уже джинсы в том же стиле. На самом деле он заказал столько кроссовок, чтобы примерить и выбрать только одни. Что делает наивная модель? Она действует тупо как автодополнение: она прекрасно предсказывает, что дальше будут белые кроссовки, хотя по факту они были как единый action и по-хорошему модель должна была обучиться связывать кроссовки с джинсами в том же стиле.

Что это значит формально? Есть ли универсальный способ диагностировать, что сплит плохой?

# Variance and randomness

# Statistical significance
# Effect size / practical significance

# Multiple comparisons

# Experimental design under constraints

# How to know whether an experiment is feasible before running it

# Pilot experiments

# Choosing the minimum experiment that can distinguish hypotheses

# Resource / compute budget

# Changing Anything Changes Everything

# On Over-ﬁtting in Model Selection and Subsequent Selection Bias in Performance Evaluation

# LLM as a judge

# 6 Lessons Learned at Booking.com

# Demystifying evals for AI agents
