Project 1 - Measuring reefs
================
Elizabeth Madin
2019-06-05

Summary:
--------

This module focuses on measuring and comparing coral patch reefs in the field and with satellite and aerial imagery of various spatial resolutions.

We're using this exercize as a means to understand the general implications of satellite imagery spatial resolution on measuring features of interest. However, it has real-world applications in terms of coral reef area measurement (e.g., Madin and Madin (2015) *Conservation Biology* and <https://allencoralatlas.org>)).

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

Materials
---------

-   transect tapes: 1 x 100m or 2x 30m per group
-   slates: 2
-   printed metadata sheet
-   mesh bag(s) to carry everything

Protocols
---------

Each group of participants will focus on a unique set of patch reefs:

-   Group 1: Patch reefs (PR): 19 (small), 16 (med), 12 (large)
-   Group 2: Patch reefs (PR): 20 (small), 22 (med), 15 (large)
-   Group 3: Patch reefs (PR): 21 (small), 23 (med), 24 (large)

#### Part 1: Field measurements

Preparation:

-   Brainstorm, plan, and practice measurements on land:
    -   Perimeter only
-   Revise plan and write protocol for field measurements
-   Create datasheets on waterproof paper
-   Gather remaining supplies for morning field trip

Measuring reefs:

-   Measure each study reef based on methods in protocol
-   Record data (including metadata - e.g., date/time, depth, etc.) on datasheet(s)
-   Make sure not to leave any gear in the water!

Data entry:

-   Open the .csv datasheet template ("Module1\_MeasuringReefs\_template.csv")
    -   Do not add/delete columns since we will combine datasets later
    -   Re-save file with your initials appended to the end of the filename (e.g., "Module1\_MeasuringReefs\_EPM.csv")
-   Choose one person from each group to enter the group's field data
    -   All others should delete all rows where column "method" = "field"
    -   For the group's data enterer, enter field data into this datasheet
    -   The column headings you’ll be filling in are:
        -   reef\_no
        -   perimeter\_m
        -   area\_m2 (use the formula =((C2/(2*PI()))^2)*PI() to calculate this from perimeter)
        -   date
        -   observer (as your three or four initials)
        -   notes (if needed)

#### Part 2: Imagery measurements

Getting started:

-   Open .kmz/.kml patch reef placemark file ("Sites.kmz") by dragging into Google Earth
-   Open .csv datasheet you saved with your initials
    -   Column headings you’ll be filling in are:
        -   reef\_no
        -   perimeter\_m
        -   area\_m2
        -   observer (as your three or four initials)
        -   notes (if needed)

Measuring reefs:

-   You will measure three of the patch reefs in Kane’ohe Bay for:
    -   Perimeter
    -   Area
        -   only in Google Earth; for Planet, use the formula =((C2/(2*PI()))^2)*PI() to calculate area from perimeter)
-   Do three replicates of each reef
-   You will use both Google Earth and Planet Explorer to measure reefs using imagery spanning a range of spatial resolutions

1.  **Google Earth**

    -   Create a folder in My Places (Add -&gt; Folder); give it a name that makes sense (eg, "KBay patch reefs")
        -   Keep this folder highlighted from now on while you're measureing reefs so the measurements will go straight into that folder
    -   Measure each of the study reefs for the following dates/spatial resolutions by using the Time Slider to select the following dates’ imagery:

        | Date (yyyymmdd) | Resolution (m) | Satellite                             | Provider     |
        |-----------------|----------------|---------------------------------------|--------------|
        | 20130115        | 0.15           | NA; aerial imagery                    | Unknown      |
        | 20130822        | 0.50           | WorldView-1/2, GeoEye-1, or Quickbird | DigitalGlobe |
        | 20110108        | ~1.00          | Ikonos                                | DigitalGlobe |
        | 20030412        | ~2.00          | EarlyBird-1 (?)                       | DigitalGlobe |

    -   Use the polygon measurement tool to extract area/perimeter
    -   Manually copy measurements into .csv
    -   Save measurement: name as “PR\#\# \_ \#.\#\# \_ \#\# \_ \#\#” = PR\[reef \#\] \_ \[resolution, in m\] \_ \[replicate\] \_ \[your initials\] (e.g., “PR21\_0.15\_01\_EM”)
    -   If any of your measurments show up in Temporary Places, drag saved measurements to the folder you created in My Places
    -   Frequently save My Places! (File -&gt; Save -&gt; Save My Places)
    -   *Note*: if you need to go back to measurements, right-click on outlines (or their corresponding saved names in My Places) -&gt; Get Info

2.  **Planet Explorer**

    -   Draw a rectangular AOI (area of interest) to cover Kane’ohe Bay
    -   Visually compare the Google Earth placemarks with the Planet Explorer AOI to locate your study reefs
    -   Measure each of the study reefs for the following satellites/dates/spatial resolutions by using the left-hand options area to select the following imagery:

        | Date (yyyymmdd) | Resolution (m) | Satellite                            | Provider |
        |-----------------|----------------|--------------------------------------|----------|
        | 20190316        | ~3.00          | PlanetScope (formerly Dove CubeSats) | Planet   |
        | 20160208        | 5.00           | RapidEye                             | Planet   |
        | 20180307        | ~10.00         | Sentinel-2                           | ESA      |
        | 20190328        | 30.00          | Landsat 8                            | USGS     |

    -   To find this imagery most efficiently, set the following search parameters:
        -   Make sure you’re in “Browse” mode
        -   Date range (right under search box) = 2016/01/01 - today
        -   Drop down menu = Daily imagery
        -   Cloud cover = 0-10%
        -   Area coverage = 90-100%
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
-   Creat a new project-specific repository in Github
-   Link your Github repo with your project directory (folder)
-   Commit/push to the new project-specific repository you created in Github

If time permits for merging and analysis of group data:

-   Send your repo's link to the rest of the group via our Slack rotation group channel
-   Pull (download) everyone else’s datasets
-   Merge others’ datasets with your dataset
-   Commit/push revised (merged) dataset to your Github repo
-   Once everyone’s data is merged, create a new R Markdown (.Rmd) file in R Studio
-   Make some basic plots to help you explore any patterns in the data
-   Run some statistical analyses to determine sources of variance, any significant trends, etc.

Do some plots tolook at patterns in the data (here are a few basic ones to get you started):

*Note: you'll need to change the data source file path & file name to match your own, and your results will be different as a result.*

``` r
################################################
# explore patterns
################################################

# Effect of method
plot(area_m2~method, data=data, na.ignore=TRUE, col="lightgrey",
     ylab="Patch reef area (m^2)", 
     xlab="Method", 
     main="Area versus method")
```

<img src="MeasuringReefs_files/figure-markdown_github/data explore-1-1.png" style="display: block; margin: auto;" />

``` r
dev.copy(pdf,"figs/method_area_effect.pdf")    # can change to .png, etc.; can change size to incr resolution
dev.off()

# Effect of imagery resolution
plot(area_m2~imagery_resolution_m, data=data, col="slategrey",
     xlim=c(0,10),
     xlab="Imagery spatial resolution (m)", 
     ylab="Patch reef area (m^2)", 
     main="Area versus imagery resolution")
res.area.lm=lm(area_m2 ~ imagery_resolution_m, data=data)
abline(res.area.lm, col = "black")
```

<img src="MeasuringReefs_files/figure-markdown_github/data explore-1-2.png" style="display: block; margin: auto;" />

``` r
summary(res.area.lm)
dev.copy(pdf,"figs/resolution_area_effect.pdf")    
dev.off()

plot(perimeter_m~imagery_resolution_m, data=data, col="slategrey",
     xlim=c(0,10),
     xlab="Imagery spatial resolution (m)", 
     ylab="Patch reef perimeter (m)", 
     main="Perimeter versus imagery resolution")
res.perim.lm=lm(perimeter_m ~ imagery_resolution_m, data=data)
abline(res.perim.lm, col = "black")
```

<img src="MeasuringReefs_files/figure-markdown_github/data explore-1-3.png" style="display: block; margin: auto;" />

``` r
summary(res.perim.lm)
dev.copy(pdf,"figs/resolution_perimeter_effect.pdf")    
dev.off()

# Effect of date (i.e., do patch reefs measureably grow or shrink over time?)
plot(area_m2~as.numeric(year), data=data, col="slategrey",
     xlab="Year", 
     ylab="Patch reef area (m^2)", 
     main="Area versus year")
date.area.lm=lm(area_m2 ~ as.numeric(year), data=data)
abline(date.area.lm, col = "black")
```

<img src="MeasuringReefs_files/figure-markdown_github/data explore-1-4.png" style="display: block; margin: auto;" />

``` r
summary(date.area.lm)
dev.copy(pdf,"figs/date_area_effect.pdf")    
dev.off()
```

Now, let's see if there's anything going on with time when imagery resolution is considered:

``` r
################################################
# analyze data
################################################

# Effects of imagery resolution + year
res.year.lm=lm(area_m2 ~ imagery_resolution_m * as.numeric(year), data=data)
summary(res.year.lm)
```

Or reef identity (number):

``` r
################################################
# analyze data
################################################

# Effects of imagery resolution + reef ID
res.reefID.lm=lm(area_m2 ~ imagery_resolution_m * reef_no, data=data)
summary(res.reefID.lm)
```

If time **doesn't** permit merging and analysis of group data:

-   Discuss as a group any patterns that seemed to emerge...e.g.,
    -   Which method you found to be more variable among groups/individuals - field or imagery?
    -   How did imagery resolution affect your measureemnts?
    -   What are the trade-offs between field vs imagery measurements?
    -   What are the trade-offs between the different imagery a) platforms and b) resolutions?
    -   Skip "Part IV: Write-up"

Part IV: Write-up
-----------------

-   When you’re finished with your analyses, go back and give each figure a short caption
-   Structure your .Rmd file as a ‘mini-paper’ with a bit of very brief text (~2-5 sentences) for each of the usual paper sections:
    -   Introduction (summarize what you’re doing with this mini-project)
    -   Methods (what you did, both in the field and the lab)
    -   Results (here’s where your figures and stats outputs will go)
    -   Discussion (mention any interesting findings and, if you have time, briefly relate this to any previous literature using a similar approach/asking similar questions)
-   This exercise will help you see the value of using R Markdown to write papers (if you’re not already familiar with or using it).
