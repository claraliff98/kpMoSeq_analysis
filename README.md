# kpMoSeq_analysis
Analyze and plot kpMoSeq dataframes

This code assumes that you have already run kpMoSeq (https://keypoint-moseq.readthedocs.io/en/latest/) and have generated the following files from your data:
- moseq_df
- stats_df
It is helpful to save these dfs as csv files as a checkpoint after finishing kpMoSeq so you don't have to rerun those models and can quickly read in your data.

It generates the following plots:
- a pointplot of relative frequency of syllables for two groups
- correlation plots of syllable frequency and a behavioral phenotype (requires an excel or csv file assigning a phenotype value for each subject/video)
- kde and histogram plots of x position occupancy for multiple groups
- kde plots for syllable usage as a function of x position, for multiple groups

This code also utilizes other excel/csv files containing experiment metadata for analyses specific to our experimental questions.For example, to explore associations between syllable usage and other behavioral phenotypes, one section of the code generates correlation plots for syllable frequency and a phenotype of interest (avoidance index). Additionally, our videos were of mice navigating at three-chamber assay, with a stress-associated odor flowing from an odor port in one of the side chambers. This code reads in and utilizes information like the position of the odor port in each video in order to analyze and visualize syllable usage across groups as a function of the mouse's distance from the source of the odor.