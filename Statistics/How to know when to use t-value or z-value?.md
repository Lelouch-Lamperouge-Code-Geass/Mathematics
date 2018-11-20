### T-score vs. z-score: When to use a t score

The general rule of thumb for when to use a t score is when your sample:

* Has a sample size below 30,  
* Has an unknown population standard deviation.  

You must know the standard deviation of the population and your sample size should be above 30 in order for you to be able to use the z-score. Otherwise, use the t-score.  

<img src="https://www.statisticshowto.datasciencecentral.com/wp-content/uploads/2013/08/t-score-vs.-z-score.png">

### T-Score vs. Z-Score: Z-score

Technically, z-scores are a conversion of individual scores into a standard form. The conversion allows you to more easily compare different data; it is based on your knowledge about the population’s standard deviation and mean. A z-score tells you how many standard deviations from the mean your result is. You can use your knowledge of normal distributions (like the 68 95 and 99.7 rule) or the z-table to determine what percentage of the population will fall below or above your result.

<img src="https://www.statisticshowto.datasciencecentral.com/wp-content/uploads/2013/09/The_Normal_Distribution.svg_1.png">

The z-score is calculated using the formula:

```
z = (X-μ)/σ
``

Where:

* σ is the population standard deviation and
* μ is the population mean.

The z-score formula doesn’t say anything about sample size; The rule of thumb applies that your sample size should be above 30 to use it.

### T-Score vs. Z-Score: T-score

Like z-scores, t-scores are also a conversion of individual scores into a standard form. However, t-scores are used when you don’t know the population standard deviation; You make an estimate by using your sample.

```
T = (X – μ) / [ s/√(n) ].
```

Where: s is the standard deviation of the sample.

If you have a larger sample (over 30), the t-distribution and z-distribution look pretty much the same. Therefore, you can use either. That said, if you know σ, it doesn’t make much sense to use a sample estimate instead of the “real thing”, so just substitute σ into the equation in place of s:

```
T = (X – μ) / [ σ/√(n) ]
```

This makes the equation identical to the one for the z-score; the only difference is you’re looking up the result in the T table, not the Z-table. For sample sizes over 30, you’ll get the same result.
