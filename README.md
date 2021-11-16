
### Analytics

Descriptive Statistics (Find the dots)
* Identify important elements
* Missing values
    * Delete records
        * significantly reduce size 
        * introduce significant bias
    * Imputation
        * average
        * interpolate from nearby values
        * predict missing values
        * method:
            * hot-deck ( last observation carried forward )
            * mean substitution (weaking correlation)
            * fit model to predict missing column 
    
    * Outliers
        * differ significantly from other data points 
        * method:
            * identify outliers (univariate)
                * distance from mean 
                  * ```\bar{x} = \frac{X_1 + X_2 + ... + X_n}{n}```
                  * describing univariate data
                    * variation 
                        * range = Xmax - Xmin (describe dispersion in data)
                    * variance (to summarize set of data points )
                    <img src="image/1.jpg">
                * distance from fitted line (points are far away from fitted line can be considered outliers)
            * coping with outliers
                * drop outliers - error in measurement
                * cap/floor maximum or minimum
                * set outlier to mean

Inferential Statistics (Connect the dots)
* Explain those elements via relationships

---

### References

1. https://www.codecogs.com/latex/eqneditor.php
2. http://mathurl.com/