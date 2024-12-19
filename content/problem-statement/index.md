cat << 'EOF' > content/problem-statement/index.md
---
title: Problem Statement
date: "2023-11-28"
---

## Introduction
This project, co-advised by Dr. Yolanda Gil, uses Natural Language Processing (NLP) techniques to analyze voluminous Diablo Canyon Independent Safety Committee (DCISC) annual reports. Our goal is to identify the role and contribution of "Traits of a Healthy Nuclear Safety Culture," as defined by the Nuclear Regulatory Commission and the Institute of Nuclear Power Operations, in incident causation.

## Motivation
Nuclear power is a viable clean energy source that generates power without pollution. The Diablo Canyon nuclear power plant, our project's focus, is the last operating nuclear power plant in California. Given the tragic incidents at Chernobyl (1986) and Fukushima (2011), ensuring this plant's safe operation until its scheduled closing in 2030 is crucial.

## Problem for the Semester
Our objectives include:
- Identifying issue statements in the 32nd annual report
- Creating a golden standard by manually labeling statements using ten healthy traits from the INPO report
- Building automated labeling models with reasonable performance
- Comparing baseline models with LLM approaches to establish groundwork for future development

## Use Case Scenario
Our system serves researchers investigating:
- Diablo Canyon Nuclear Power Plant's healthy traits
- Year-over-year performance comparisons
- Areas for future improvements

Researchers can analyze reports from the 21st to 33rd annual reports, generating:
- Lists of healthy traits for each year
- Statistical analyses
- Visualizations for better understanding of key issues
- Trend comparisons for leadership performance
- Identification of persistent safety concerns
EOF