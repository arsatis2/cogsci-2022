# Modeling Causal Inference from Emotional Displays

This GitHub repository contains the source code and data analysis for the CogSci 2022 submission, titled "Modelling Causal Inference from Emotional Displays".

## Source Code for Inference Models

The inference models were implemented in Python, using the [pymc3](https://docs.pymc.io/en/v3/) package.

> Multiple Causes Model

This model describes how people infer the likely cause of an outcome (i.e., a light bulb turning on) after being shown a sequence of actions performed by a cartoon agent. Multiple candidate causes were possible to explain the given outcome and the model combines information from the environmental as well as the character's actions and emotional displays to infer causality. The source code for this model can be found [here](cog-sci-present-model/Emotion%20Causal%20Learning%20Model%20(Multiple-Causes).ipynb).

> Multiple Outcomes Model

This model describes how people infer the likely causal effect(s) of an action in a scene where multiple outcomes were possible (i.e., multiple light bulbs). Similar to earlier, this model combines information from the environmental as well as the character's actions and emotional displays to infer causality. The source code for this model can be found [here](cog-sci-present-model/Emotion%20Causal%20Learning%20Model%20(Multiple-Outcomes).ipynb).

## Data Analyses

Our results and analyses are documented in the [cog-sci-present-analysis](cog-sci-present-analysis) folder. This includes the statistical tests and model comparisons which were reported in the paper. There are three subfolders:

* [multiple-causes-scenario](cog-sci-present-analysis/multiple-causes-scenario): contains files for the first study, i.e., where a multiple-causes scenario was examined.
* [multiple-causes-scenario-tracking](cog-sci-present-analysis/multiple-causes-scenario-tracking): contains files for the follow-up of the first study, i.e., examination of causal inferences at _key moments_ of the scene.
* [multiple-outcomes-scenario](cog-sci-present-analysis/multiple-outcomes-scenario): contains files for the second study, i.e., where a multiple-outcomes scenario was examined.

Three files are present within each of these subfolders, namely:

* ecl\_dat.csv: contains the anonymized data of participants' responses (used for analysis).
* \<study name\>-analysis.html: our results and analyses on the data.
* \<study name\>-analysis.Rmd: our raw analyses on the data.
