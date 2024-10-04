---
layout: page
title: DPhil Project
description: Investigating the use of wrist-worn accelerometry to predict Parkinson's disease
img:
importance: 1
category: work
related_publications: true
---

Parkinson's disease (PD) is a growing public health concern with rising diagnoses and no preventive treatments.
Early-stage monitoring is crucial for understanding disease progression and smartwatches offer great potential in continuous real-world monitoring.
This DPhil thesis explores the use of wrist-worn accelerometers to predict future PD diagnoses.

In the initial phase of this work, I reviewed literature on PD and wearable monitoring technologies.
This review highlighted research into walking pattern monitoring and proposed risk prediction models using accelerometer data.
To conduct this research, a variety of datasets were used, including those from the UK Biobank Physical Activity Monitoring, PPMI-Verily, Capture-24, OxWalk, and MJFF Levodopa Response studies.

Wrist-worn accelerometer data depended on the development of reliable activity classification models for this thesis' aims.
Existing models were improved to detect labels of activity intensity labels (sleep, sedentary, light, and moderate-vigorous activity) using a self-supervised ResNet-18 model.
When trained and evaluated on the Capture-24 dataset, this model achieved a median macro F1 score of 0.861, outperforming the existing model's score of 0.780.
Walking recognition models were also enhanced to be trained on both healthy and PD datasets.
Patterns were observed showing that walking recognition models trained only on healthy participants performed worse in participants within increasing severity of PD.
However, training the same models on both healthy and PD data improved general performance, with no drop in performance for higher severities of PD.

An epidemiological analysis was then conducted to investigate the association between device-measured daily step count and PD incidence in the UK Biobank, to assess low daily steps as a risk factor for PD.
A 1,000-step increase in median daily steps resulted in a hazard ratio of 0.92 for PD diagnosis, consistent after accounting for various confounders.
However, this association attenuated to null after removal of the first six years of follow-up, giving an indication of reverse-causation driving this association.
Daily steps therefore appears to be a predictor of, but not a risk factor for PD.

Models trained to categorise activity intensity and walking were subsequently employed to compare active walking windows among participants with varying PD statuses.
In the PPMI-Verily dataset, a self-supervised ResNet-18 model distinguished between diagnosed PD, prodromal PD, and healthy controls, achieving a macro F1 of 0.586 and AUROC of 0.856 using the active walking windows.
This finding establishes that differences in walking behaviour related to PD impairment can be detected by wrist-worn accelerometers.

The final phase of research combined a variety of digital measures extracted to build risk prediction models for PD in the UK Biobank.
These wrist-worn accelerometer-derived digital measures were compared with traditional risk factors.
The most effective risk model incorporated a PD gait score, which compared detected active walking windows of participants to those of diagnosed PD participants in the PPMI-Verily dataset.
This model produced a c-index of 0.883, compared to 0.786 when using non-accelerometer-based traditional risk factors for PD.
These results highlight the added benefit of wrist-worn accelerometry, particularly PD-specific digital measures, for improving PD prediction models.

In summary, this thesis leverages wrist-worn accelerometry and machng to predict PD, aiming to enahnce early diagnosis and monitoring.
The results across the different studies support the promising use of wearable technoine learnilogy for PD monitoring.
