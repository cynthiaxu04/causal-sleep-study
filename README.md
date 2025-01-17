# Causal Inference: Effects of Visible Light on Sleep Quality

## Problem & Motivation
Sleep is fundamental to maintaining general health and cognitive performance. We are interested in the effect of visible light on sleep quality from artificial light sources such as indoor lights and electronic devices. Prior studies have found that visible light exposure prior to bedtime can suppress the onset of melatonin production, which can impact sleep quality [3]. Previous studies on light exposure before sleep have predominantly focused on the effect of blue light emitted by electronic devices. We seek to study if limiting all visible light with the simple use of sunglasses can improve sleep quality in adults.  

Our research question is thus posed: **does reducing exposure to visible light by wearing sunglasses one hour before bedtime have an impact on sleep quality?**  

We theorize sunglasses limit exposure to visible light, and when worn in the runup to bedtime, mimic a more natural onset of darkness, potentially triggering the biological processes that prepare the brain for sleep. We hypothesize that reducing light exposure before bedtime by wearing sunglasses will have a positive effect on sleep quality.  

We pose the null hypothesis to state that **sunglasses worn before bedtime have no effect on sleep quality.** Our alternative hypothesis is that the intervention has either a positive or negative impact on sleep quality. We account for the potential for sunglasses to negatively impact sleep.  

## Data & Approach

In this experiment, we tested the intervention of wearing sunglasses for an hour before bedtime on subject sleep quality. To measure sleep quality, we utilized sleep score features provided by common consumer activity trackers. We configured a paired design to compare control vs. treatment phase sleep scores of subjects.  

We enrolled 22 subjects on a rolling basis to participate in 2 weeks of study per subject. Using paired design, each subject experienced a control and treatment phase lasting Monday through Thursday night of each week. We randomly assigned subjects to either complete the control or treatment phase first to account for any potential order effects. For example, the first participant enrolled was assigned “treatment-control” (i.e., treatment phase for week 1, then control phase for week 2). The second enrolled participant was assigned “control-treatment”, the third “treatment-control”, etc.  

During both control and treatment phases, subjects were instructed to follow their regular bedtime routines while wearing their activity trackers to sleep. In the treatment phase, however, subjects were instructed to also wear sunglasses an hour before bedtime. To encourage compliance and discourage attrition, Subjects were offered a $20 Amazon gift card for completion.

At the end of each phase, participants were asked to report:
1. their sleep scores for the 4 nights
2. treatment compliance (if during treatment phase)
3. subjective rating of their quality of sleep
4. subjective rating of how easily they fell asleep

## Key Learnings
> **Participants did not experience a statistically significant effect on sleep quality as measured by sleep score while wearing sunglasses before bed.**

When examining our results on an individual participant level, we find substantial variation by individual. It is thus clear that for any future studies, we would recommend collecting much more extensive health and lifestyle information on participants, increasing the duration of treatment and control measurement periods, and increasing the sample size to account for variance in the population.

> **The dependent variable and covariates that we examined in this study do not sufficiently explain the observed variation in our outcome of sleep score.**

To estimate average treatment effect, we observe a statistically insignificant coefficient on sunglasses treatment of -0.56 with a robust standard error 3.22, implying that our treatment of wearing sunglasses before bedtime, as administered, does not have an impact on sleep quality as measured by sleep score.  

In our subsequent models, we add additional covariates to regress on. Prior to the study, participants were surveyed to rate their sleep quality, trouble sleeping, and total sleep duration. Our model that includes this “Previous Sleep Info” shows that both historical sleep quality and the total usual number of hours slept per night, as reported by participants, are predictive of sleep score: the standard error of sunglasses treatment decreases. Similarly, in our next model that includes demographic information from participants, mainly age group and gender, we observe that age group is a significant predictor of sleep score. Specifically, lower sleep quality is correlated with a higher age. This improvement in regression is also reflected in the increasing R-squared and F-statistic values as more covariates are added.  

## References
1. Blume, C., Garbazza, C., & Spitschan, M. (2019). Effects of light on human circadian rhythms, sleep and mood. Somnologie, 23(3), 147.
2. Diekelmann S. Sleep for cognitive enhancement. Front Syst Neurosci. 2014 Apr 2;8:46. doi: 10.3389/fnsys.2014.00046. PMID: 24765066; PMCID: PMC3980112.
3. Gooley JJ, Chamberlain K, Smith KA, Khalsa SB, Rajaratnam SM, Van Reen E, Zeitzer JM, Czeisler CA, Lockley SW. Exposure to room light before bedtime suppresses melatonin onset and shortens melatonin duration in humans. J Clin Endocrinol Metab. 2011 Mar;96(3):E463-72. doi: 10.1210/jc.2010-2098. Epub 2010 Dec 30. PMID: 21193540; PMCID: PMC3047226.
4. Pham, H. T., Chuang, H. L., Kuo, C. P., Yeh, T. P., & Liao, W. C. (2021, August). Electronic device use before bedtime and sleep quality among university students. In Healthcare (Vol. 9, No. 9, p. 1091). MDPI.
5. Owusu-Marfo, J., Lulin, Z., Antwi, H. A., Kissi, J., Antwi, M. O., & Asare, I. (2018). The Effect of Smart mobile devices usage on Sleep Quality and academic performance–A Narrative Review. Canadian Journal of Applied Science and Technology, 6(2).
