Module 1 - Measuring reefs
================
Elizabeth Madin
2019-05-02

Summary
-------

This module focuses on measuring and comparing coral patch reefs in the field and with satellite imagery of various spatial resolutions.

Goals
-----

-   Make connection between use of field data and remote (e.g., satellite; aerial) imagery to measure biological/habitat variables
-   Highlight strengths and limitations of each approach
-   Start thinking about ?s to ask/answer in a) course project and b) own research
-   Provide coral reef field experience
-   Generate dataset for potentially publishable study (?)

Components
----------

-   Devise/practice field measurement protocol
-   Measure reefs in-situ
-   Measure reefs w/satellite imagery of various spatial resolutions via:
-   Google Earth
-   Planet Explorer
-   Compare measurement variability based on method, imagery spatial resolution, etc.

Results
-------

Let's do some basic plots:

<img src="Module1_MeasuringReefs_files/figure-markdown_github/data explore-1-1.png" style="display: block; margin: auto;" /><img src="Module1_MeasuringReefs_files/figure-markdown_github/data explore-1-2.png" style="display: block; margin: auto;" />

    ## 
    ## Call:
    ## lm(formula = area_m2 ~ imagery_resolution_m, data = data)
    ## 
    ## Residuals:
    ##     Min      1Q  Median      3Q     Max 
    ## -160.99  -58.21   25.15   61.08  105.32 
    ## 
    ## Coefficients:
    ##                      Estimate Std. Error t value Pr(>|t|)    
    ## (Intercept)           715.811     21.936  32.632  < 2e-16 ***
    ## imagery_resolution_m   41.435      4.918   8.426  6.6e-09 ***
    ## ---
    ## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1
    ## 
    ## Residual standard error: 83.46 on 26 degrees of freedom
    ##   (8 observations deleted due to missingness)
    ## Multiple R-squared:  0.732,  Adjusted R-squared:  0.7216 
    ## F-statistic:    71 on 1 and 26 DF,  p-value: 6.596e-09

<img src="Module1_MeasuringReefs_files/figure-markdown_github/data explore-1-3.png" style="display: block; margin: auto;" />

    ## 
    ## Call:
    ## lm(formula = perimeter_m ~ imagery_resolution_m, data = data)
    ## 
    ## Residuals:
    ##      Min       1Q   Median       3Q      Max 
    ## -14.3041  -4.7745   0.6426   5.5838  11.3959 
    ## 
    ## Coefficients:
    ##                      Estimate Std. Error t value Pr(>|t|)    
    ## (Intercept)           97.8752     1.8938  51.682  < 2e-16 ***
    ## imagery_resolution_m   3.8329     0.4245   9.028  1.7e-09 ***
    ## ---
    ## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1
    ## 
    ## Residual standard error: 7.206 on 26 degrees of freedom
    ##   (8 observations deleted due to missingness)
    ## Multiple R-squared:  0.7582, Adjusted R-squared:  0.7489 
    ## F-statistic: 81.51 on 1 and 26 DF,  p-value: 1.704e-09

<img src="Module1_MeasuringReefs_files/figure-markdown_github/data explore-1-4.png" style="display: block; margin: auto;" />

    ## 
    ## Call:
    ## lm(formula = area_m2 ~ as.numeric(year), data = data)
    ## 
    ## Residuals:
    ##     Min      1Q  Median      3Q     Max 
    ## -309.13 -114.35  -57.88  101.90  374.95 
    ## 
    ## Coefficients:
    ##                   Estimate Std. Error t value Pr(>|t|)
    ## (Intercept)      -7378.043  12367.992  -0.597    0.555
    ## as.numeric(year)     4.080      6.141   0.664    0.512
    ## 
    ## Residual standard error: 174.6 on 30 degrees of freedom
    ##   (4 observations deleted due to missingness)
    ## Multiple R-squared:  0.0145, Adjusted R-squared:  -0.01835 
    ## F-statistic: 0.4414 on 1 and 30 DF,  p-value: 0.5115

Now, let's see if there's anythign going on with time when imagery resolution is considered:
