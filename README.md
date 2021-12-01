
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
                      <img src="image/2.jpg">
                      
                    * variance Bessel's correction ( improve our estimate of variance by -1 denominator) 
                    <img src="image/3.jpg">
                    * standard deviation (Square root of variance)  
                    <img src="image/4.jpg">
                * distance from fitted line (points are far away from fitted line can be considered outliers)
                    * outliers may be the data points that do not fit into same relationship the rest of the data 
            * coping with outliers
                * drop outliers - error in measurement
                * cap/floor maximum or minimum
                * set outlier to mean
                * method:
                    * erroneous observation
                    * scrutinizing outliers 
                    * standardize data 
                        * subtract mean the data points and divide std 

Inferential Statistics (Connect the dots)
* Explain those elements via relationships

---

### Data Cleansing

* Remove duplicates -> Data Tab
* Remove blank -> Home -> Filter 
* Highlight blank -> Home -> Find & Select -> Go to Special -> Blank
    * Fill blank -> Ctrl + Enter
* Identify outliers
    * zscore : (x - xbar)/std 
    * anything greather than 3 or lower than -3 std is outliers 

### Excel
```
1. mean : avg
2. standard deviation : stdev
3. zscore : standardize(<col>,mean,std) 
            STANDARDIZE(C2,$U$21,$U$22)
4. 2 method :
    set outlier not greater than 3 or less than 3
    * filter zscore
    IF(OR(D2<$N$23,D2>$O$23),"",D2)
    * clamped zscore
    IF(F2<$N$23,$N$23,IF(F2>$O$23,$O$23,F2))
```

### References

1. https://www.codecogs.com/latex/eqneditor.php
2. http://mathurl.com/