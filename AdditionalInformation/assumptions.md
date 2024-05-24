# Assumptions and more

Before doing any analysis you need to check if you can even do this type of analysis! **If you do not check these assumptions, the outcome of your test does not mean anything!** Hence, it is crucial to do these before doing the analysis! As these assumption checks are often forgotten, I want to shed some more light on this topic using this document. I will explain the checks you need to do and what you can do if those checks fail.

## Tests

### T-Test

Requirements:
- IV is discrete and nominal
- At most 2 groups, otherwise ANOVA
- DV is continuous

Assumptions:
- Indepence of samples within groups: See [Independence](#independence)
- Independence of samples between groups: If not, then Paired T-Test
- Normality within groups: Use **Shapiro-Wilk test** and visually inspect using QQ-plots and/or histogram. If fail, see [Normality](#normality)
- Homogeneity of variances between groups: Use **Levene's test**. If fail, see [Homogeneity of variances](#homogeneity-of-variances)

### Univariate ANOVA (One-way, Two-way, Factorial)

Requirements:
- IV's are discrete and nominal
- DV is continuous

Assumptions:
- Independence of samples within groups: See [Independence](#independence)
- Independence of samples between groups: If not, then Repeated Measures ANOVA
- Normality within groups: Use **Shapiro-Wilk test** and visually inspect using QQ-plots and/or histogram. If fail, see [Normality](#normality)
- Homogeneity of variances: Use **Levene's test**. If fail, see [Homogeneity of variances](#homogeneity-of-variances)

### Repeated Measures Univariate ANOVA (One-way, Two-way, Factorial)

Requirements:
- IV's are discrete and nominal
- DV is continuous

Assumptions:
- Independence of samples within groups: See [Independence](#independence)
- Same participants in each group
- Balanced design: every participant has **exactly** the same number of measurements
- Normality within groups: Use **Shapiro-Wilk test** and visually inspect using QQ-plots and/or histogram. If fail, see [Normality](#normality)
- Sphericity: Use **Mauchly's test**. If fail, see [Sphericity](#sphericity)

### Multivariate ANOVA (One-way, Two-way, Factorial)

Requirements:
- IV's are discrete and nominal
- DV's are continuous

Assumptions:
- Independence of samples within groups: See [Independence](#independence)
- Independence of samples between groups: If not, then Repeated Measures MANOVA
- Multivariate normality within groups: Not easily tested, so testing normality for each DV separate using **Shapiro-Wilk test** is adviced. If fail, see [Normality](#normality)
- Homogeneity of variances: Use **Levene's test**. If fail, see [Homogeneity of variances](#homogeneity-of-variances)
- Homogeneity of covariance matrices: Use **Box's test**. If fail... we do not really know what to do. The effect of violating this is unclear.

### Repeated Measures Multivariate ANOVA  (One-way, Two-way, Factorial)

Requirements:
- IV's are discrete and nominal
- DV's are continuous

Assumptions:
- Independence of samples within groups: See [Independence](#independence)
- Same participants in each group
- Balanced design: every participant has **exactly** the same number of measurements
- Multivariate normality within groups: Not easily tested, so testing normality for each DV separate using **Shapiro-Wilk test** is adviced. If fail, see [Normality](#normality)
- Homogeneity of variances: Use **Levene's test**. If fail, see [Homogeneity of variances](#homogeneity-of-variances)
- Homogeneity of covariance matrices: Use **Box's test**. If fail... we do not really know what to do. The effect of violating this is unclear.

### (Multiple) Linear/Logistic Regression

Requirements:
- IV's are discrete or continuous
- DV is continuous (only for linear regression)
- DV is discrete (only for logistic regression)

Assumptions:
- Independence of samples: See [Independence](#independence)
- Non-zero variance of IV's
- No perfect multicollinearity: No IV should be a perfect linear combination of other IV's (r < 0.9)
- Normally distributed errors: Residuals should be distributed normally
- Linearity: The relationship between the IV's and DV is assumed to be linear

## Details

### Independence
Independence of samples within groups is an assumption for almost every test except for a Repeated Measures (M)ANOVA. Independence is a vague term that basically boils down to the question if all samples are equally independent of each other. For example, imagine you measure a participant multiple times (say 10 times) and do this for 10 participants. In the end you obtain a dataset with 100 datapoints. Are these samples all independent from each other? No, because measurements taken from the same participant tend to be more equal (share more information) than measurements taken from two different participants. Despite this, seemingly, trivial explanation, many studies ignore this detail and often conduct T-Tests and ANOVA's on many thousands of datapoints. The result is that your test will more likely turn out to be signficiant while it actually isn't. In fact, studies have shown that with 10 observations per participant, your chance of finding a significant relation is **inflated by 15x**! This Type I error comes from the fact your test thinks there are much more independent samples (participants) than there actually are! 

If you fail this assumption, there are two things you can do. Either you switch to a Repeated Measures test, or you aggregate your data to the extent it becomes independent. A Repeated Measures test only allows us to check for within-subject effects. If you are mostly interested in between-subject effects, you would have to perform a Mixed (M)ANOVA which allows you to measure both within and between-subject effects. If you are only interested in between-subject effects, aggregation is your best option. In our example of our 10 participants, this would mean we would aggregate each participant's datapoints into one datapoint, leaving us with 10 independent datapoints in the end. Remember that this aggregation does not necessarily has to be the average value. There are many ways you can aggregate a variable.

### Normality
All tests except regression assume the DV(s) follow a Normal distribution within each category/group. If your IV consists of three levels/groups, the DV must be normally distributed within each of these three groups. This sounds like a very strict assumption, but in reality (M)ANOVA's are designed to be fairly robust to non-normally distributed data up to a certain extent. Of course, your data cannot be extremely skewed, but slight violations are accepted. 

If you fail the assumption of normality, you can do two things. You either use a data transformation to deskew/scale the data or you choose to do a non-parametric test. Deskewing the data can be done by using lower powers if your data is right/positively skewed (square root, natural log) and higher powers when your data is left/negatively skewed (squared, cube).

### Homogeneity of variances
The two-sample T-Test and ANOVA both assume a homogeneity of variances. Or in other words, that the variance of your DV is roughly equal within each group. Violating this assumption does not seem to affect the test much if your group sizes are equal. However, if this is not the case, the importance of homogeneity of variances rises with the unequality of your groups. The effect of violation can then go both ways. If the largest group has a larger variance than the others, the ANOVA will less likely turn out to be significant whereas in reality there would have been a significant effect. If the variance is smaller than the others, the ANOVA will more likely turn out to be significant (type I error).

If you fail this assumption, you can correct for the magnitude of this violation by using the Brown and Forsythe F-ratio. This controls the effect of the largest group and seems to work pretty well when homogenity of variances was not met. 

### Sphericity
Sphericity extends the concept of homogeneity of variances to a repeated measures design. It basically assumes that there is equal variance between of the pairwise differences between the different measurements of each participant. Consequently, sphericity can only be checked whenever there are more than 3 repeated measures. Otherwise, there is only one variance in difference between the two repeated measures. Due to this reason, some argue that a Repeated Measures design should include at least 3 repeated measures. In fact, that makes sense as a repeated measures design with only two measurements is basically a paired T-Test. 

If sphericity is violated, people often control for this violation instead of doing another test or transforming the data. You control for sphericity by the use of two methods. The Greenhouse-Geisser correction or the Huynh-Feldt correction. The first one is best to use when sphericity is severly violated (sphericity < 0.75) while the latter is less conservative when sphericity is only slightly violated (sphericity > 0.75). Both methods correct the F-statistic and you can use either of them to use this correction.


