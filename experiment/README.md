# HumanEval: Odd-One-Out Task Experiment
# Experiment Scripts

## Overview
This folder contains the code required to run the experiment. The experiment uses [JsPsych] to present stimuli and record responses.

Created by Frieda Born in January 2024.

## jsPsych
The experiment uses jsPsych v7.3.3 (https://www.jspsych.org/7.3/). jsPsych is a JavaScript library for creating and running behavioral experiments in a web browser. Some of the base scripts for the jsPsych plugins where customized to accommodate additonal functionality needed to run the experiment. Changes are made transparent in comments within the plugin codes.

## Experiment Structure

- `index.js`: The main file that runs the experiment. It integrates the jsPsych library to present stimuli and collect responses from participants.
- `jspsych/`: A directory containing all jsPsych library plugins used to design and run the experiment. Please note that some plugins where customized.
- `experiment_preparation` Folder that holds preparatory scripts for the experiment.
  - `Subsetting_experiment_subjects.ipynb`: This script preapres .csv files for testing on the ARC servers. The output of this script can be found in the server_inputs folder.
- `server_inputs/`: .csv files that define the trial structure and experimental stimuli used.
- `stimuli/`: In the original experiment, this folder housed all the stimuli used in the experiment, managed with Large File Storage (LFS) to handle the size and quantity efficiently. In this repository, we are not providing all images used in the experiment, as LSF can't be used here. All the stimuli names are, however, documented in the *server_inputs*.csv file. So, for running the experiment, one can filter for these stimuli in the ImageNet Dataset and run the experiment.
  - `consent_form/`: Contains materials related to the consent form that participants must agree to before participating in the experiment.
  - `instructions/`: Includes visualizations used for instructions for participants on how to proceed with the experiment.
  - `catch_trials/`: Contains *gold standard triplets* used as catch trials to ensure participants pay attention throughout the experiment.
    -  `catchTrialData.js `: defining the catch-trial structure.
  -  `stim/`: additional stimuli to run the experiment, like placeholders
  -  `training_trials/`: trials that are used to familiarize participants with the task.
    -  `training_trials.js `: defining the structure of the training trials.


### Prerequisites

- The JsPsych library set-up on you computer (only if you want to develop yourself)
- Any modern web browser (e.g., Chrome, Firefox, Safari), for accessing the task.
- Helpful: an editor (like visual studio code, where this experiment was developed) (also only if you want to work with the code of this exp.)
