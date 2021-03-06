# Sketching Sounds: Using sound-shape associations to build a sketch-based sound synthesiser 

This is the repository related to my PhD research at the Centre for Digital Music at Queen Mary University of London.

## Abstract
Humans are surprisingly good at creating mental images of sound, however current tools rarely accommodate a perception-centered production approach that allows for a straightforward realisation of sound ideas. While research has found commonalities in how humans describe sound across various modalities, this research focuses on the crossmodal associations between sound and visual shapes and how they can be used to drive sound synthesis. The results will be used to build a functioning sketch-based sound synthesiser. Based in the field of music psychology and music computing, this research also touches on the fields of interaction design, human-computer interaction and musical interfaces.

For a quick overview, please have a look at this [website](https://sfrl.github.io/PhD_Research_Sketching_Sounds/Webpage/).

## Study 1.1 - Sketching Sounds: An exploratory study on sound-shape associations 

### Introduction
This study aims to discover how participants represent different sounds visually using a simple digital drawing interface. 28 participants (14 female) were presented with 10 different sounds and were asked to draw whatever they believe represented the sound best. Sounds were chosen to represent different timbral characteristics (brightness, noisiness, warmth etc.) and sources (synthesisers, acoustic instruments and abstract textures). Each of the 10 sounds was repeated during a study run, leading to a total of 20 sketches per participant. Sketches were categorised by 6 participants (4 female) in a card sorting exercise.  

### Results
The results show that the participants' sketches show some commonalities. While some participants use figurative images (e.g. a piano or a cello) to describe a sound, most chose abstract representations. Objective features like corner or curve points were extracted from these abstract sketches to find possible correlations with audio features. The results showed correlations that align with existing body of sound-shape research.

|<img src="Stage_1/Images/Spearman.png" width="600px"/>|<img src="Stage_1/Images/Categories_Music_Pro.png" width="600px"/>
|:--:|:--:|
*Spearman’s rank correlation coefficients between sketch and audio features with annotated p-values: p<.05 (\*), .01 (\*\*), .001 (\*\*\*)*|*Absolute category counts by music proficiency*|

### Material

The study setup can be found [here](https://sfrl.github.io/PhD_Research_Sketching_Sounds/Stage_1/Study1_part1/Study_setup/).

The Jupyter notebook containing the analysis of the card sorting analysis can be found [here](https://github.com/SFRL/PhD_Research_Sketching_Sounds/blob/master/Stage_1/Study1_part1/Card_Sorting_Analysis.ipynb)

The Jupyter notebook containing the data analysis including more graphs can be found [here](https://github.com/SFRL/PhD_Research_Sketching_Sounds/blob/master/Stage_1/Study1_part1/Sketching_Sounds_an_exploratory_study_analysis.ipynb).

The sketches have been compiled into an interactive gallery, including the sounds, that can be explored [here](https://sfrl.github.io/PhD_Research_Sketching_Sounds/Stage_1/Study1_part1/Sketch_Gallery/).

## Study 1.2 - Seeing Sounds, Hearing Shapes

### Introduction
This study takes abstract sketches from study 1 part 1 and presents them to participants in a quiz-like game. Participants hear a sound and have to find the "right" sketch from 4 different options. The aim of this study is to find out if these sketches can successfully communicate the characteristics of a sound.

### Results
This study is ongoing and does not have any results yet.

### Material
The design for study 1 part 2 can be found [here](https://phd-studies-eddd5.web.app/). 


## Study 2: Creating a sound-sketch dataset

### Study 2.1 - Interface Evaluation 

Results from study 1 show that similar sound-shape associations exist between participants. However, the large variety of sketches make it difficult to quantise sketches in a precise manner, especially in regards to a working synthesis application. In a series of small studies, multiple development iterations of the drawing interface are tested to find an interface configuration that limits the user input to homogenise sketches between participants while still allowing enough variance for creative expression. 

The current iteration allows users to only draw one stroke within a defined length. The study can be accessed [here](https://sketching-sounds.web.app/)

### Study 2.2 - Creating a sound-sketch dataset

The main part of study 2 will revolve around creating a controlled, large dataset (~150 participants) of sound-sketches using the interface developed during study 2.1. The dataset will be used to train a neural network based on the [Sketch-RNN](https://magenta.tensorflow.org/sketch-rnn-demo) architecture that will be able to predict sound characteristics based on the sketch input. 


