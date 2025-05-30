# 🧠  HumanEval: Odd-One-Out Task Experiment

Created by Frieda Born in January 2024.

This repository contains the code used in the online behavioural experiment "HumanEval".
This study is being conducted by the Adaptive Memory and Decision Making group at the Max Planck Institute for Human Development in collaboration with BIFOLD at TU Berlin.

## Overview

**HumanEval** is an online experiment designed to study Human alignment, which is becoming central to representation learning (e.g., Muttenthaler et al. 2023, Sucholutsky et al., 2023): We seek models that go beyond excelling solely in machine learning downstream tasks; our goal is to develop models that align closely with human perception and intentions. To accomplish this objective, with this study, we aim to collect a set of human odd-one-out similarity judgments to evaluate whether (synthetically generated) similarity judgments of existing state-of-the-art human-aligned models (Muttenthaler et al., 2023) correspond to ground-truth human judgments. This assessment will provide insights into whether there is a disparity between model and human object similarity spaces and pinpoint the specific areas of divergence.

To gather human similarity judgments, we aim to employ the **odd-one-out task**. This task is a commonly used task in the cognitive sciences to measure human notions of object similarity without biasing a participant in a specific direction (Hebart et al., 2020; Muttenthaler et al., 2022, 2023). In this task, images are presented to a participant, and the participant selects the image that is least similar to the other two. The odd-one-out task has been used to study properties of human mental representation for many decades (e.g., Fukuzawa et al., 1988; Robilotto & Zaidi, 2004; Hebart et al., 2020). Compared to tasks involving numerical/Likert-scale pairwise similarity judgments, the odd-one-out task does not require subjects to interpret the scale similarly to one another, and does not require that the degree of perceived similarity is cognitively accessible.

## Repository Structure
- `analysis/`: Scripts and notebooks for data analysis. These are the scripts:
    - `data_preprocessing.ipynb` : Script to remove participant identifiable information from the raw data files and prepare to data release.
    - `demographic_information.ipynb`: Script analysing the demographic information of the participants.
    - `stats_eval.ipynb` Script that holds statistical tests and visualization.
- `experiment/`: Code for running the experiment, including stimuli and experiment scripts, preparation of experiment, ect. Please also find a separate `README.md` about the experiment here.
- `docs/`: Documentation and references for the project.
    - `Variable_codebook_Levels`: Variable codebook giving an overview of all the variables (and variable levels) used in the study.

## Data Access
The data is hosted on [GIN](). Instructions for accessing the data and using the data files is also provided on GIN.

## Getting Started

- The experiment was be accessed via a public link of the form: "https://967-humaneval-164.exp.amd.mpib.org/"(not active anymore, as the experiment was deactivated on public servers after data collection was completed).

### Prerequisites

- The JsPsych library set-up on your computer (only if you want to develop yourself)
- Any modern web browser (e.g., Chrome, Firefox, Safari), for accessing the task.
- Helpful: an editor (like visual studio code, where this experiment was developed) (also only if you want to work with the code of this exp.)

### License

[MIT]

### Acknowledgments of supervision for this project

- Lukas Muttenthaler, Bernhard Spitzer, Klaus Greff, Michael C. Mozer, Klaus Robert Müller, Thomas Unterthiner, Andrew Lampinen, Katherine Hermann, Robert Geirhos

## Contact

For questions about this experiment or repository feel free to contact: born[at]mpib-berlin.mpg.de

