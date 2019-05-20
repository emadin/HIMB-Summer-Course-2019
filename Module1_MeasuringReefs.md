Module 1 - Measuring reefs
================
Elizabeth Madin
2019-05-19

Summary
-------

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
-   Clone repository <https://github.com/emadin/HIMB-Summer-Course-2019-Remote-Sensing-Imagery-Module-1-Measuring-Reefs->, which will allow you to open the .csv datasheet template ("Module1\_MeasuringReefs\_template.csv")
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

-   Download .kmz/.kml patch reef placemark file ("Sites.kmz"") from <https://github.com/emadin/HIMB-Summer-Course-2019-Remote-Sensing-Imagery-Module-1-Measuring-Reefs->
-   Open saved .csv datasheet template adn re-save with your initials appended to the end of the filename (e.g., "Module1\_MeasuringReefs\_EM.csv")
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

-   Create a new R Markdown (.Rmd) file
-   Make some basic plots to help you explore any patterns in the data
-   Run some statistical analyses to determine sources of variance, any significant trends, etc.
-   When you’re finished, go back and give each figure a short caption
-   Structure your .Rmd file as a ‘mini-paper’ with a bit of very brief text (~2-5 sentences) for each of the usual paper sections:
    -   Introduction (summarize what you’re doing with this mini-project)
    -   Methods (what you did, both in the field and the lab)
    -   Results (here’s where your figures and stats outputs will go)
    -   Discussion (mention any interesting findings and, if you have time, relate this to any previous literature using a similar approach/asking similar questions)
-   This exercise will help you see the value of using R Markdown to write papers (if you’re not already familiar with or using it)

Now, let's do some basic plots to get you started:

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

Useful information
------------------

#### Determining resolution of Google Earth imagery

There is no tool that will tell you the resolution of Google Earth's imagery in any specific location...but, you can:

-   look at the copyright info to get an idea (e.g., it's from DigitalGlobe, then it's most often 0.5m)
-   use rules of thumb (below) about what size of objects you can see clearly

#### Summary of providers, satellites & resolutions in Google Earth

These are at least the main types found in Google Earth, though this list is not necessarily exhaustive:

        Provider          | Instrument      | Spatial resolution (m) | Operational   
        ----------------- | --------------- | ---------------------- | ------------  
        US Geolog. Survey | Landsat         | 30 (15 pan-sharpened)  | LS1 from 1972; LS8 from Feb 2013 
        SpotImage         | SPOT 1-7        | 10 - 2.5               | Mar 1998 – present 
        Digital Globe     | EarlyBird-1     | 3                      | DigitalGlobe 
        Digital Globe     | Ikonos          | ~1                     | DigitalGlobe  
        Digital Globe     | WorldView-1/2   | ~0.5                   | Unknown       
        Digital Globe     | GeoEye-1        | ~0.5                   | DigitalGlobe  
        Digital Globe     | Quickbird       | ~0.5                   | DigitalGlobe  
        Airbus            | Pleiades        | ~0.5                   | DigitalGlobe  
        Digital Globe     | WorldView-3     | ~0.3                   | Unknown       
        Various           | Aerial systems  | ~0.15                  | DigitalGlobe  
        Various           | Cameras on kites| A few cm               | Varies 

#### Summary of providers, satellites & resolutions in Planet Explorer

These are the only types currently found in Planet Explorer:

        Provider          | Instrument      | Spatial resolution (m) | Operational   
        ----------------- | --------------- | ---------------------- | ------------  
        US Geolog. Survey | Landsat-8       | 30 (15 pan-sharpened)  | Feb 2013-present
        ESA (Eur Space Agency)| Sentinel-2  | 10                     |  
        Planet            | EarlyBird-1     | 5                      |  
        Planet            | Ikonos          | ~3                     |   
        Planet            | WorldView-1/2   | 0.72                   |        

#### Rules of thumb for determining spatial resolution of satellite imagery

from GIS Stack Exchange, answered by Christiaan Adams of Google Earth Outreach; <https://gis.stackexchange.com/questions/11395/spatial-resolution-of-google-earth-imagery/256850>)

The resolution of imagery in Google Earth varies depending on the source of the data. When you zoom out, you will see the nice, pretty global coverage produced from a mosaic of many Landsat scenes, which have a native resolution of ~30m (~15m pan-sharpened).

Zooming in, you'll start to get high-resolution in most places. There are many rural areas, especially in Africa, where broad coverage is provided by the SPOT satellites, which produce anywhere from 10m to 1.5m resolution. Next you can still find some Ikonos data in a few places, at about 1m resolution. Then you get down to the really high-resolution satellites, including Digital Globe's WorldView-1/2/3 series, GeoEye-1, and Airbus' Pleiades, all of which provide data at around 0.5m resolution. That's about the limit for satellite data, though a few places are staring to get data from newer satellites (including WorldView-3) at around 0.3m.

In much of North America, Europe, Japan and some other places, you'll find even higher resolution images which generally come from aerial systems (cameras on airplanes), and a lot of that data in Google Earth is at about 0.15m resolution. Finally, there are just a few tiny spots around the world where Google Earth shows data collected by citizen scientists (through the Public Lab), using cameras on kites and balloons, which can get down into the few centimeters per pixel range.

There is no tool that will tell you the resolution of Google Earth's imagery in any specific location.

Here are some fun rules of thumb I use to quickly estimate the resolution of what I'm looking at, by zooming in on cars. If roads and house roofs look like they are 2-5 pixels wide, then you are probably seeing SPOT's 5m or 2.5m products. If you can clearly make out the shapes of cars, but their windshields are poorly defined, then it might be 1m from Ikonos. If the windshield is pretty clear, but you can only barely (or not quite) make out the frame pillars along the sides of the windshield, then you're probably looking at 0.5m satellite imagery. If you can clearly make out the pillars, and start to see the side-view mirrors on the car, then you're most likely looking at aerial data in the 0.15m range. More generally, find an object that you know the approximate size of, and see about how many pixels it's covered by, and do the math.

There is a good suggestion in previous answers, that you zoom way in and look at the copyright strings, as that will often tell you at least what company the data came from (as well as the acquisition date listed in the status bar)... though for the aerial data that may not help as a copyright is often not listed. If it's from DigitalGlobe, then it's most often 0.5m. If you really want to dig in, you can go to the company's online imagery catalog, look in your desired location, search for images around the date provided, and try to find an image that looks the same (similar colors, cloud patterns, etc.). If you can find the corresponding image in the catalog, then you can see all the metadata, including which satellite and what resolution.

#### Problems I've encountered in Google Earth

-   Date mismatches between TimeSlider and "Imagery date" (info at bottom right of image): e.g., 12/30/2008 on time slider says 12/31/2007 on bottom

-   Same images given for multiple dates (e.g., 7/30/2006 on time slider is same image as 12/30/2008 on time slider) - this one also has mismatched "Imagery date"

-   Different dates coming up on Time Slider for same image during different Google Earth sessions (i.e., image of PR 21 and area has come up on Time Slider for both 8/10/2014 and 4/30/2015, yet neither date appears as an option on Time Slider when the other date is given for the image) – see screenshots below. Note that both images have date 8/10/2014 in “Imagery Date” field at bottom of image. Note (tiny) Time Slider dates at top left of each image:

<center>
<img src="info/DateMismatch_1.png" alt="Note Time Slider date at top" style="width:90.0%" /> <img src="info/DateMismatch_2.png" alt="Note Time Slider date at top" style="width:90.0%" />

</center>
