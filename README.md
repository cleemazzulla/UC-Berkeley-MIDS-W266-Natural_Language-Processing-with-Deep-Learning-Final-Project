# Neural Metrics for Machine Translation

## Authors
- Courtney Mazzulla ([cleemazzulla@berkeley.edu](mailto:cleemazzulla@berkeley.edu))
- Tynan Prasad ([prasadtyrnan@berkeley.edu](mailto:prasadtyrnan@berkeley.edu))
- Julian Rippert ([jrippert@berkeley.edu](mailto:jrippert@berkeley.edu))

## Abstract
This project provides an in-depth analysis of machine translation (MT) metrics, techniques, and trade-offs associated with their usage. We propose a neural network-based approach to replicate features that human raters use during their assessments, achieving notable performance with a lightweight model architecture.

## Introduction
Advancements in neural network architectures and methodologies have improved machine translation (MT) task performance. Our project focuses on the evaluation metrics for MT and proposes improvements over existing metrics like BLEU and ROUGE.

## Key Contributions
1. Fine-tuning the top-performing model checkpoint on MQM data.
2. Implementing data augmentation techniques to enhance performance.
3. Developing a feature engineering approach to outperform the fine-tuned BLEURT model using a lightweight feed-forward neural network.

## Skills Mastered
- **Machine Learning**: Understanding and implementing various machine learning models, including neural networks and regression models.
- **Data Augmentation**: Techniques like synonym substitution and sentence reordering to enhance model robustness.
- **Feature Engineering**: Extracting explicit features from language pairs to improve model performance.
- **Natural Language Processing (NLP)**: Working with text data, understanding translation quality, and evaluating translation systems.
- **Model Fine-Tuning**: Enhancing pre-trained models for specific tasks and data sets.
- **Performance Evaluation**: Using metrics like Pearson correlation to assess model performance against human judgment.
- **Data Analysis**: Analyzing data sets to establish baselines and identify areas for improvement.

## Data Sets
- **Direct Assessments (DA)**: Absolute scores or labels given by humans.
- **Scalar Quality Metric (SMQ)**: Segment-level scalar ratings with document context.
- **Multidimensional Quality Metric (MQM)**: Metric based on an error hierarchy including Accuracy, Fluency, Terminology, Style, and Locale.

## Methodology
### Data Augmentation
- **Synonym Substitution**: Replacing a randomly selected token with semantically similar words.
- **Sentence Re-ordering**: Shuffling sentences to introduce noise and help with overfitting.

### Baseline and Experiments
- Establishing a baseline using the BLEURT-20-D6 model checkpoint.
- Implementing data augmentation and fine-tuning to enhance performance.

### Feature Engineering
- **Mutation Strings**: Categorizing errors into deletions, insertions, or substitutions.
- **Feature Analysis**: Analyzing features for predictive power before training models.

## Results
- Models trained on feature sets like token counts, engram overlaps, and mutation counts showed varying degrees of success in predicting MQM scores.
- Combining all features under one model provided a comprehensive evaluation, although separate models for different languages could further improve results.

## Conclusion
Our project demonstrates the potential of feature engineering in developing neural metrics for MT. We also highlight the limitations and future directions for improving translation quality assessment.

## Acknowledgements
Special thanks to our instructors Mike Tamir, PhD, and Paul Spiegelhalter, PhD, for their consultation, proof-reading, feedback, and continued support.

## References
- Freitag et al., 2022. Results of WMT22 Metrics Shared Task: Stop Using BLEU – Neural Metrics Are Better and More Robust.
- Sellam, Das, and Parikh, 2020a. BLEURT: Learning robust metrics for text generation.
- Rolnick, Veit, and Belongie, 2017. Deep learning is robust to massive label noise.
