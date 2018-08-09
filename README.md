# ERP_habituation
ERP habituation modelling code relative to:

Mancini F, Pepe A, Bernacchia A, Di Stefano G, Mouraux A, Iannetti GD. (2018)
Characterising the short-term habituation of event-related evoked potentials.
eNeuro

Written in Matlab R2016b by F Mancini, fm456@cam.ac.uk


'wilcoxon_clustercorr.m' performs a point-by-point, one-sample Wilcoxon signed-rank test of EEG waveforms is. Please see details at the beginning of the code.

The script to model the habituation of EEG data is 'svd_analysis.m'. It requires the Curve Fitting Toolbox in Matlab.

'svd_analysis' loads data from matrix 'wave_data.mat' then calls a number of sub-functions to perform the following processing steps:

1. Singular value decomposition of the EEG matrix
2. Estimate SVD significance
3. Modelling of the right-singular vectors (habituation components)
4. Compare decay models according to BIC
5. Estimate p-values of winning models using resampling statistics
6. Make figure of winning models for each rank and condition
7. Make figures of SVD results

For more details see comments embedded in 'svd_analysis.m'

Preprocessed EEG data are available at 
