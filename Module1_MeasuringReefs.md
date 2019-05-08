Module 1 - Measuring reefs
================
Elizabeth Madin
2019-05-08

Summary
-------

This module focuses on measuring and comparing coral patch reefs in the field and with satellite and aerial imagery of various spatial resolutions.

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
-   Compare patterns and measurement variability based on method, imagery spatial resolution, etc.
-   Write up results as 'mini-paper'

Protocols
---------

Each group of participants will focus on a unique set of patch reefs:

-   Group 1: Patch reefs (PR): 19 (small), 16 (med), 12 (large)
-   Group 2: Patch reefs (PR): 20 (small), 22 (med), 15 (large)
-   Group 3: Patch reefs (PR): 21 (small), 23 (med), 24 (large)

#### Part 1: Field measurements

Preparation:

-   Brainstorm, plan, and practice measurements on land:
    -   Area
    -   Perimeter
-   Revise plan and write protocol for field measurements
-   Download .csv datasheet template ("Module1\_MeasuringReefs\_template.csv") from <https://github.com/emadin/HIMB-Summer-Course-2019-Remote-Sensing-Imagery-Module-1-Measuring-Reefs->
    -   Do not add/delete columns since we will combine datasets later
    -   Column headings in red are those you’ll be filling in
-   Print datasheets (relevant columns) on waterproof paper
-   Gather remaining supplies for morning field trip

Measuring reefs:

-   Measure each study reef based on methods in protocol
-   Do three replicate measurements per reef
-   Record data on datasheet(s)
-   Make sure not to leave any gear in the water!

Data entry:

-   Enter data into downloaded datasheet template

#### Part 2: Imagery measurements

Getting started:

-   Download .kmz/.kml patch reef placemark file (Sites.kmz) from <https://github.com/emadin/HIMB-Summer-Course-2019-Remote-Sensing-Imagery-Module-1-Measuring-Reefs->
-   Open saved .csv datasheet template
    -   Column headings in red are those you’ll be filling in

Measuring reefs:

-   You will measure three of the patch reefs in Kane’ohe Bay for:
    -   Area
    -   Perimeter
-   Do three replicate measurements per reef
-   You will use both Google Earth and Planet Explorer to measure reefs using imagery spanning a range of spatial resolutions

1.  **Google Earth**

    -   Measure each of the study reefs for the following dates/spatial resolutions by using the Time Slider to select the following dates’ imagery:

        | Date (yyyymmdd) | Resolution (m) | Satellite                             | Provider     |
        |-----------------|----------------|---------------------------------------|--------------|
        | 20130115        | 0.15           | NA; aerial imagery                    | Unknown      |
        | 20130822        | 0.50           | WorldView-1/2, GeoEye-1, or Quickbird | DigitalGlobe |
        | 20110108        | 1.00           | Ikonos                                | DigitalGlobe |
        | 20030412        | 2.00           | EarlyBird-1 (?)                       | DigitalGlobe |

    -   Use the polygon measurement tool to extract area/perimeter
    -   Manually copy measurements into .csv
    -   Save measurement: name as “PR\#\# \_ \#.\#\# \_ \#\# \_ \#\#” = PR\[reef \#\] \_ \[resolution, in m\] \_ \[replicate\] \_ \[your initials\] (e.g., “PR21\_0.15\_01\_EM”)
    -   Drag saved measurements to My Places
    -   Frequently save My Places (File -&gt; Save -&gt; Save My Places)
    -   *Note*: if you need to go back to measurements, right-click on outlines (or their corresponding saved names in My Places) -&gt; Get Info

2.  **Planet Explorer**

    -   Draw a rectangular AOI (area of interest) to cover Kane’ohe Bay
    -   Visually compare the Google Earth placemarks with the Planet Explorer AOI to locate your study reefs
    -   Measure each of the study reefs for the following satellites/dates/spatial resolutions by using the left-hand options area to select the following imagery:

        | Date (yyyymmdd) | Resolution (m) | Satellite                             | Provider     |
        |-----------------|----------------|---------------------------------------|--------------|
        | 20130115        | 0.15           | NA; aerial imagery                    | Unknown      |
        | 20130822        | 0.50           | WorldView-1/2, GeoEye-1, or Quickbird | DigitalGlobe |
        | 20110108        | 1.00           | Ikonos                                | DigitalGlobe |
        | 20030412        | 2.00           | EarlyBird-1 (?)                       | DigitalGlobe |

    -   To find this imagery most efficiently, set the following search parameters:
        -   Make sure you’re in “Browse” mode
        -   Date range (right under search box) = 2016/01/01 - today
        -   Drop down menu = Daily imagery
        -   Cloud cover = 0-10%
        -   Area coverage = 0-90%
        -   Source = tick sources corresponding to “satellite” above
        -   *Tip*: do this satellite by satellite for faster searching
    -   Use the “measure area” tool to extract area
    -   Use the “measure distance” tool to extract perimeter (hold shift for free hand measurement of both area/perim)
    -   Manually copy measurements into .csv
    -   *Note*: there’s no way to save measurements, so double-check each entry for accuracy before moving on

Part 3: Data analysis
---------------------

Once all data is collected:

-   Check your dataset for any typos, missing values, etc.
-   Commit/push to Github
-   Pull (download) everyone else’s datasets
-   Merge others’ datasets with your dataset
-   Commit/push revised (merged) dataset to Github

Once everyone’s data is merged:

-   Create a new R Markdown file
-   Make some basic plots to help you explore any patterns in the data
-   Run some statistical analyses to determine sources of variance, any significant trends, etc.
-   When you’re finished, go back and give each figure a short caption
-   Structure your .Rmd file as a ‘mini-paper’ with a bit of very brief text (~2-5 sentences) for each of the usual paper sections:
    -   Introduction (summarize what you’re doing with this mini-project)
    -   Methods (what you did, both in the field and the lab)
    -   Results (here’s where your figures and stats outputs will go)
    -   Discussion (mention any interesting findings and, if you have time, relate this to any previous literature using a similar approach/asking similar questions)
-   This exercise will help you see the value of using R Markdown to write papers (if you’re not already familiar with or using it)

Let's do some basic plots to get you started:

<img src="Module1_MeasuringReefs_files/figure-markdown_github/data explore-1-1.png" style="display: block; margin: auto;" /><img src="Module1_MeasuringReefs_files/figure-markdown_github/data explore-1-2.png" style="display: block; margin: auto;" /><img src="Module1_MeasuringReefs_files/figure-markdown_github/data explore-1-3.png" style="display: block; margin: auto;" /><img src="Module1_MeasuringReefs_files/figure-markdown_github/data explore-1-4.png" style="display: block; margin: auto;" />

Now, let's see if there's anything going on with time when imagery resolution is considered:

``` r
################################################
# analyze data
################################################

# Effects of imagery resolution + year
res.year.lm=lm(area_m2 ~ imagery_resolution_m * as.numeric(year), data=data)
summary(res.year.lm)
```

    ## 
    ## Call:
    ## lm(formula = area_m2 ~ imagery_resolution_m * as.numeric(year), 
    ##     data = data)
    ## 
    ## Residuals:
    ##     Min      1Q  Median      3Q     Max 
    ## -148.53  -50.92   20.52   45.47  114.43 
    ## 
    ## Coefficients:
    ##                                        Estimate Std. Error t value
    ## (Intercept)                           29220.705  17736.667   1.647
    ## imagery_resolution_m                  -4500.815   7563.176  -0.595
    ## as.numeric(year)                        -14.165      8.806  -1.609
    ## imagery_resolution_m:as.numeric(year)     2.256      3.750   0.601
    ##                                       Pr(>|t|)
    ## (Intercept)                              0.112
    ## imagery_resolution_m                     0.557
    ## as.numeric(year)                         0.121
    ## imagery_resolution_m:as.numeric(year)    0.553
    ## 
    ## Residual standard error: 74.95 on 24 degrees of freedom
    ##   (8 observations deleted due to missingness)
    ## Multiple R-squared:  0.8005, Adjusted R-squared:  0.7755 
    ## F-statistic:  32.1 on 3 and 24 DF,  p-value: 1.449e-08

``` r
## START HERE: why only one predictor variable showing up in output??
```

Useful information
------------------

#### Determining resolution of Google Earth imagery

There is no tool that will tell you the resolution of Google Earth's imagery in any specific location...but, you can: \* look at the copyright info to get an idea (e.g., it's from DigitalGlobe, then it's most often 0.5m) \* use rules of thumb (below) about what size of objects you can see clearly

#### Summary of providers, satellites & resolutions in Google Earth

These are at least the main types found in Google Earth, though this list is not necessarily exhaustive:
