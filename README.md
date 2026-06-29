# Childcare Interaction Dataset

Evaluation dataset for the paper:

> **From CCTV to Social Interaction: An F-formation-based Interaction Analysis in Childcare Environments**
>
> Suchun Park, Mi Yeon Park, Hyunin Cho, Kyungphil Ryoo, Jihwan Kim, Youngjung Uh, Hyoun K. Kim, Kyoungwoo Lee
>
> *IEEE International Conference on Advanced Video and Signal-Based Surveillance (AVSS), 2026*

## Overview

This dataset provides evaluation benchmarks for two tasks in real-world childcare CCTV environments, collected at an operational childcare facility across three days of free play activity (approximately 5.2 hours total).

## Tasks

### Task 1: Person Re-Identification (Re-ID)

Matching detected person crops to a pre-registered frontal photo gallery under uniform-wearing conditions.

- **Gallery**: Frontal reference photographs per child per day
- **Query**: Detection crops extracted from CCTV frames
- **Annotations**: 10,144 ground-truth identity labels across 3 evaluation days
- **Metric**: Top-1 identification accuracy

### Task 2: Interaction Detection

Determining per-frame pairwise social interactions from geometric cues (interpersonal distance + body orientation) grounded in F-formation theory.

- **Frames**: Sampled CCTV frames from free play periods
- **Calibration**: Homography matrices for ground-plane projection (pixel to world coordinates)
- **Annotations**: 18,526 frame-level pairwise interaction labels across 3 evaluation days
- **Expert validation**: 4,630 expert-coded pairwise observations using OSRAC-P behavioral coding
- **Metrics**: Precision / Recall / F1-score (per-frame), Spearman rank correlation (cumulative)

## Data Release

The dataset is currently under preparation for public release. 
This page will be updated with download links upon availability.

For early access or collaboration inquiries, please contact us at the email below.

## Citation

If you use this dataset, please cite:

```bibtex
@inproceedings{park2026cctv,
  title     = {From CCTV to Social Interaction: An F-formation-based
               Interaction Analysis in Childcare Environments},
  author    = {Park, Suchun and Park, Mi Yeon and Cho, Hyunin and
               Ryoo, Kyungphil and Kim, Jihwan and Uh, Youngjung and
               Kim, Hyoun K. and Lee, Kyoungwoo},
  booktitle = {Proc. IEEE International Conference on Advanced Video
               and Signal-Based Surveillance (AVSS)},
  year      = {2026}
}
```

## Contact

**Suchun Park** — suchun.park@yonsei.ac.kr
