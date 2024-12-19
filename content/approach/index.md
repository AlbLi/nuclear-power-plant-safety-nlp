---
title: "Approach and Methodology"
date: "2023-12-19"
---

## Data Processing Pipeline

### Data Quality Assessment
- Raw Annual Reports extracted from [DCISC website](https://www.dcisc.org/annual-reports/)
- Focus on the 32nd Annual Report
- Manual extraction and labeling of issue statements using INPO Traits
- Mixed input formats (text and images) requiring OCR processing
- Challenges with scattered issue statements and incomplete descriptions

### Data Preprocessing Steps
1. OCR Implementation
   - Python-based OCR for image-to-text conversion
   - Generation of machine-readable text files
2. Data Preparation
   - Manual extraction and labeling for golden standard dataset
   - Vectorization of issue statements and safety traits
   - Enhanced seed word development based on previous work

## Model Development

### Seed Word Model
- **Technologies**: spacy, scikit-learn
- **Implementation**:
  - Classic NLP approach with baseline 53% accuracy
  - Enhanced with weighted safety traits
  - Added comprehensive seed word sets
  - F1 score: 47%

### Logistic Regression Model
- **Technologies**: scikit-learn
- **Features**:
  - Text vectorization for large-scale analysis
  - 10-fold cross-validation implementation
  - Performance evaluation across multiple metrics

### Large Language Models
- **Models**: ChatGPT3.5, Claude-2
- **Process**:
  - Fine-tuned with INPO safety culture traits
  - Structured output format:
    - Original/summarized issue statement
    - Trait labels with confidence levels
    - Classification reasoning
  - [ChatGPT3.5 Model Documentation](https://chat.openai.com/share/34046a4f-ca87-4311-8fcb-6b1b83764578)

## Model Evaluation Framework
- Primary Metrics:
  - Accuracy
  - F1 Score
- Validation Methods:
  - Cross-validation for overfitting prevention
  - Performance comparison across models
