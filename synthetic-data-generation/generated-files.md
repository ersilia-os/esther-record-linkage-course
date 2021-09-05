---
description: >-
  This page contains several pre-computed datasets to be used throughout the
  workshop
---

# Precomputed datasets

{% hint style="info" %}
Please [contact Miquel Duran-Frigola](mailto:miquel@ersilia.io) if you are not satisfied with the current datasets!
{% endhint %}

Below, you can find several exemplary precomputed synthetic datasets. Each zipped folder contains a source file, a target file, a ground truth file in CSV format. Parameters used for the calculation are given in JSON format.

## S01: Toy example

This small dataset has 10 samples in the source file and 100 samples in the target file. The expected linkage rate is high \(90%\).

{% file src="../.gitbook/assets/s01.zip" %}

## S02: Realistic CIDRZ dataset

This dataset is representative of a typical facility-to-SmartCare linkage as performed at CIDRZ. The size of the source file is 5,000 samples and the size of the target file is 50,000. Repeated visits and duplicates are added. The expected linkage rate is 70%.

{% file src="../.gitbook/assets/s02 \(1\).zip" %}

## S03: Large clean dataset

This dataset is aimed at testing the computational performance of the linkage pipeline. The source file has 50,000 samples and the target file has 500,000 samples. The expected linkage rate is 80%. No significant noise was added, so the linkage is expected to be simple. Some identifiers are included in the source file.

{% file src="../.gitbook/assets/s03 \(1\).zip" %}

## S04: Mid-size noisy dataset

This dataset includes a significant amount of noise, meaning misspellings, name swappings, etc. are frequent. In addition, there is less consistency in the formats. The number of source samples is 10,000 and the number of target samples is 30,000. The expected linkage rate is 70%.

{% file src="../.gitbook/assets/s04.zip" %}

