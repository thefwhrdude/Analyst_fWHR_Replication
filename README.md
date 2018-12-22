# A Failed Attempt to Replicate He et al. (2018) - Facial Structure and Achievement Drive: Evidence from Financial Analysts- Forthcoming in Journal of Accounting Research

Notice:

***** This is not a full replication of the original paper *****

***** A full replication is impossible due to author's manual sample selection and facial annotation *****

***** We used a larger sample, and a machine-learning method (Le et al. 2012) to automatically annotate 194 points on a face and calculate fWHR *****

***** We did not find association between fWHR and Accuracy in our setting*****

***** Please interpret our result with Extreme Caution *****

Abstract:

He et al. (2018) Facial Structure and Achievement Drive: Evidence from Financial Analysts is forthcoming in Journal of Accounting Research. This paper demonstrates a positive association between 1,193 Chinese Sell-side Analysts' facial Width-to-Height Ratio, to their forecast accuracy. Even unpublished yet, this paper has been widely distributed through the internet, causing great debate in both academia and industry. Many comments point to the recent contradicting findings in the relationship between fWHR and level of testosterone in both adult male and adolescent male. Out of curiosity, we attempt to replicate this paper. A full-replication was impossible because the author manually removed about 17% of the sample due to low picture quality and they used human eyes to measure fWHR. We attempt to conduct the closest replication by using a larger sample over a longer time period, and employing a machine learning method to automatically denote the landmarks and calculate fWHR on 2,147 Chinese male analysts. Unfortunately, our attempt has failed to find any association between the fWHR and measure of their forecast accuracy. Our further attempt includes different cut-off point between high and low fWHR, and two alternative measures of accuracy, we failed to find associations either.

1.Background

He et al. (2018) https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3112471 demonstrates a positive association between 1,193 Chinese Sell-side Analysts' facial Width-to-Height Ratio, to their forecast accuracy. Since it was conditionally accepted at JAR, this paper has caused great discussion in the academia and industry. A number of social media posts was published online with more than 100,000 readership, and thousands of comments have questioned the underlying mechanism- the association between fWHR and level of testosterone (T hereafter) in male.

Readers’ questions do not come out of nowhere. After the original paper documenting the association between fWHR and T was published in Evolution and Human Behavior (https://doi.org/10.1016/j.evolhumbehav.2013.03.005), at least three papers have been published on academic journals providing contradicting findings to this association. For example, Bird et al. (2016) https://doi.org/10.1016/j.evolhumbehav.2016.03.004 find no significant positive relationship between fWHR and baseline testosterone. Hodges-Simeon et al. (2016) https://doi.org/10.1371/journal.pone.0153083 focus on T in adolescence male, a period the fWHR was formed, and find no evidence supporting this association between fWHR and T. More recently, Kosinski (https://doi.org/10.1177/0956797617716929) used survey to show that fWHR does not substantially link with any self-reported behavioral tendencies.

Given the amount of contradicting literature on the association between fWHR and T, we decided to replicate He et al. (2018) as a course project to provide additional evidence to the literature.

2.Limitations of our Replication:

A full replication was impossible due a few restrictions and we used a closest replication possible:

1.	Author downloaded all available profile pictures of analyst displayed on SAC (Security Association of China) website in July 2015, we were not able to backdate the list of available pictures on that date. Instead we used a larger sample covering 2,147 male analysts displayed at least once during January 2015 to July 2018, collected from the official website of the SAC. In theory, our sample should include the sample used in He et al. (2018), we couldn’t verify this notion unless the author release their raw data.

2.	Author used human eyes to measure the fWHR. Due to resource constraint, we were not able to do so. Instead, we used a machine-learning based method developed in computer vision provided by Le et al. (2012) to automatically annotate 194 landmarks on human face and calculate fWHR as the ratio between the width (distance between two facial boundaries) and height (distance between top of lip and highest point of eyelids). According to Le et al. (2012) this model has an accuracy of above 95% in labeling these facial landmarks. - See attached Annotated picture. 

3.	Author manually deleted 249 male analysts from their original sample (17% of original sample) and explanation was because their pictures are not clear enough. We were not able to backout this process. As a matter of fact, the machine-learning model we used did not encounter such an issue (rejected picture count for about 0.5% of our sample). Because the profile pictures provided by SAC are subject to certain standard to make sure they can be clear enough to be used for identification purpose at the certificate test centers by exam proctors.

Due to these sample differences, reader should use caution in interpreting our findings.

3.Results

The replication results are attached to this thread. We report OLS regression coefficients and robust T-statistics in all tables.

Table1: Our sample size is larger than He et al. due to the differences in replication method mentioned above. In terms of value and variance, our sample seems to be comparable to He et al. paper.

Table2: We estimate the same model as He et al. , including the same fixed effect and error clustering. We tried four measures of fWHR including the one (above median, below median) used by He et al. (2018), - raw fWHR value, median as breakpoint, 1st quartile, 1st quintile.

We did not find significant associations in any of these specifications.

Table3: We replace the dependent variable with a more intuitive measure – Absolute Forecast Error (AFE), this measure has been widely used in Accounting and Finance literature.

We did not find significant associations in any of these specifications.

Table4:We replace the dependent variable with a more concurrent measure – Proportional Mean Absolute Forecast Error (PMAFE)

We did not find significant associations in any of these specifications.

4.Conclusions

We have failed the attempt to replicate He et al. (2018) paper. But this inconsistency may be the result of different sample selecting process, and difference face annotation method. Please interpret our results with caution.
To satisfy the publication standard at JAR, we suggest the following:

1.	Author should release their raw data of fWHR for more direct replication (It won’t violate picture owners’ privacy as they have already agreed with SAC to make public disclosure of their pictures in the test agreement) 

2.	Author should show robustness by using a machine learning based, or other non-human based method to measure fWHR to eliminate potential measurement error

3.	Author should give a clearer explanation of the pictures deleted due to low quality

4.	Author should provide robustness check using other measure of forecast accuracy such as the widely used AFE (absolute forecast errors) or PMAFE (Proportional mean absolute forecast errors) in literature

5.Dataset Available for Other Users

1.	Analyst fWHR.txt – A dataset including analyst-level information and raw fWHR Variables: Brokerage of the analyst, Name of the analyst, Education level, gender, Full-name of brokerage current, fWHR

2.	Replication Result.pdf

3. Sample Annotated Picture

6.Reference

Le, Vuong, et al. "Interactive facial feature localization." European conference on computer vision. Springer, Berlin, Heidelberg, 2012.

Kosinski, Michal. "Facial width-to-height ratio does not predict self-reported behavioral tendencies." Psychological science 28.11 (2017): 1675-1682.

Lefevre, Carmen E., et al. "Telling facial metrics: facial width is associated with testosterone levels in men." Evolution and Human Behavior 34.4 (2013): 273-279.

Bird, Brian M., et al. "Does the facial width-to-height ratio map onto variability in men's testosterone concentrations?." Evolution and Human Behavior 37.5 (2016): 392-398.

Hodges-Simeon, Carolyn R., et al. "Facial width-to-height ratio (fWHR) is not associated with adolescent testosterone levels." PloS One 11.4 (2016): e0153083.

He, Xianjie and Yin, Huifang and Zeng, Yachang and Zhang, Huai and Zhao, Hailong, Facial Structure and Achievement Drive: Evidence from Financial Analysts (November 24, 2018). Journal of Accounting Research, Forthcoming. Available at SSRN: https://ssrn.com/abstract=3112471 or http://dx.doi.org/10.2139/ssrn.3112471
