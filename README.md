# STA-141A-Course-Project

## Project Overview
This repository contains the final project for STA 141A, focusing on a subset of data collected by Steinmetz et al. (2019). In the study, the experiments were performed on a total of 10 mice over 39 sessions. Each session comprised several hundred trials, during which visual stimuli were randomly presented to the mouse on two screens positioned on both sides of it. The stimuli varied in terms of contrast levels, which took values in {0, 0.25, 0.5, 1}, with 0 indicating the absence of a stimulus. The mice were required to make decisions based on the visual stimuli, using a wheel controlled by their forepaws. A reward or penalty (i.e., feedback) was subsequently administered based on the outcome of their decisions. In particular,

- When left contrast > right contrast, success (1) if turning the wheel to the right and failure (-1) otherwise.
- When right contrast > left contrast, success (1) if turning the wheel to the left and failure (-1) otherwise.
- When both left and right contrasts are zero, success (1) if holding the wheel still and failure (-1) otherwise.
- When left and right contrasts are equal but non-zero, left or right will be randomly chosen (50%) as the correct choice.

The activity of the neurons in the mice’s visual cortex was recorded during the trials and made available in the form of spike trains, which are collections of timestamps corresponding to neuron firing. In this project, we focus specifically on the spike trains of neurons from the onset of the stimuli to 0.4 seconds post-onset. In addition, we only use 18 sessions (Sessions 1 to 18) from four mice: Cori, Frossman, Hence, and Lederberg.The project involves analyzing [data description] using R, employing various statistical and visualization techniques to uncover meaningful insights.
