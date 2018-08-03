# Scalable Spectral Clustering with Cosine Similarity (ssc-cosine)

This documentation explains how to execute the Matlab codes for the algorithm presented in the following paper 
   "Scalable Spectral Clustering with Cosine Similarity", G. Chen, ICPR 2018, Beijing, China
and also indicates which scripts can be used to reproduce the results reported in the above paper.

Structure of the package
- Main function: ssc-cosine.m
- Scripts used to reproduce the results reported in the ICPR18 paper:
  * script_20news_results.m:  Table I
  * script_20news_insights.m: Figures 1,2
  * script_20news_alpha.m:    Figure 3
  * script_tdt2_top30.m:      Figure 4
  * script_digits_results.m:  Table II
- Scripts used to reproduce the results reported in the short paper:
  * script_20news_alpha_scalable3.m:    Figure 1
  * script_tdt2_top30_DMt.m:            Figure 4
  
Required external functions:
- The kmeans.m function, available through the Statistics and Machine Learning Toolbox, is needed by the main function ssc-cosine.m. If that toolbox is not available in the computer, then one may use instead a substitute kmeans implementation, such as the litekmeans.m function available at http://www.cad.zju.edu.cn/home/dengcai/Data/Clustering.html.
- The bestMap.m function, available also on the above webpage, is needed by the scripts for finding the best match between the ground-truth labels and the group labels obtained by the function ssc-cosine.m, in order to compute the clustering accuracy.

The litekmeans.m and bestMap.m functions have been included in this repository (for convenience).
