# 360 Degree Gait
Download URL: https://opendata.ljmu.ac.uk/id/eprint/133/3/Gait%20Dataset.zip

## Introduction
This dataset provides walking data for 65 diverse participants (labelled p1, p2, etc.). Participant_Anthropometry.xlsx provides the gender, height, weight, and ethnicity of each participant.

The recordings for each participant are structured in 3 experiments, each containing 6 tasks (with the participant going in the opposite direction in odd numbered tasks). Each experiment provides a different set of viewing angle with the videos labelled to include the participant number, experiment number, task number, viewing angle, for example, P1_E1T1_90 refers to participant 1, experiment 1, task 1 and 90 degree viewing angle. Additionally "_ALT" is appended to videos where participants have provided a second outfit, these are stored in "alternative clothing" folders containing in each experiment folder. 


## How to use
By default, it loads all file directory information like other datasets before training starts. If you need to use some of these data separately, such as `aligned-sils`, then you can use the `data_in_use` parameter in `data_cfg` lexicographically, *i.e.* `data_in_use: [true, false, false, false]`.
