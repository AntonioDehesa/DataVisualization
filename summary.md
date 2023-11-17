# Week 2

## Accuracy and ease of judgement of data based on visual elements

1. position
2. length
3. direction
4. angle
5. area
6. volume
7. curvature
8. lightness
9. color saturation
10. color hue

## General principles of Good Data Visualization
* Encourage comparison of elements
* Show the data
* Variation in color, shape, and line can help represent categorical information
* The incorporation of multiple visual elements, when intentional, helps represent and draw attention to components of a plot. But eliminate unnecessary visual elements
* Induce the viewer to think about the data
* Reveal the data at multiple leves from broad to fine
* Maintain a clear purpose, explanation, description/exploration, diagnosis

We often use color to represent categorical data, but consider when and to what extent its necessary. 


## Deciding on chart types
* Some experimentation and experience is helpful here
* start bi considering what you try to show: 
    * Distribution (histogram, boxplot, violin, strip plot)
    * Composition (stacked bar, pie, treemap, area)
    * Relationship (scatter, bubble, heatmap)
    * Comparison (bar, line)
    * Change (line, area, alluvial diagrams)
    * Location (maps)
    * Connection (graph visualization matrix, arc, radial)

* there is overlap here of course. Oftentimes we are addressing more than one of the above areas in a single plot or set of plots
* If a chart type makes sense within a given context then use it
* Oftentimes you can creatively extend a plotting approach into a different realm through clever data formatting and coding

## Consider the Audience

* Audience has a huge bearing on the level of detail (stylistically and
functionally) and the plot type.
* Sometimes you are the audience
    - General data exploration, assessing assumptions, evaluating models, etc.
* Academic audiences
     - Think publication
* Peer audiences
    - Fellow data scientists
* Lay audiences
    - Clients (potentially), cross-functional colleagues, general end users of a visual analysis product
* Executive audiences

## Color

* Color should be used intentionally.
* We often use it to encode categorical information.
* We also use it to represent magnitude, density, strength of relationship, divergence, etc.
* Our purpose impacts our color scheme.
    * For example, when encoding categorical information we’ll want to use a qualitative palette (different, distinguishable, maybe even meaningful colors)
* Encoding continuous information will necessitate a more sequential palette.
* As we'll see with heatmaps, sometimes a diverging color palette is appropriate.
* Categorical palettes are typically defined by hue (distinct colors). These are bad for representing numerical data.
* There are elements of both art and science in selecting colors, and there is no single best palette.
* Variations in luminance (brightness) better represent numerical information.
* Sometimes branding considerations need to be addressed.
* This [website](https://colorbrewer2.org/) is a good tool for determining color palettes.

## Some Rules of Thumb

* Bar charts should typically have the continuous axis start at zero.
* Be aware of the potential for occlusion of your information. (area charts are particularly susceptible to this.)
* Pie charts are seldom the best choice.
* Consider your axes ticks. Are you showing proportion, count, the result of applying some function (central tendency perhaps).
* Keep accessibility in mind. (For example, green and red is a poor choice of color scheme.)
* Limit color and other chart ink to what is essential for interpretation.
* If you’re using area to encode data, make sure the scale is accurate.
* Avoid 3-D representations, unless it’s necessary…it probably isn’t.
* Don’t hesitate to add narrative to your plots, especially if you have multiple plots that tell a story or sequentially unpack a phenomenon.

## Avoid Distortion

It's often recommended to avoid truncating coordinate axes in order to highlight/enhance/distort/magnify an ovservation.  When using a Cartesian coordinate system it's typically recommended to show the origin.  This is dependant on the context though.  If the audience is familar with the data in question and subtle fluctuations are meaningful, then it can be appropriate to deviate from the standard practice.

## Simpson's Paradox

This isn't a visualization phenomenon, but rather a statistical paradox that can be well-illustrated with the help of some simple plots.  A Simpson's Paradox occurs when a relationship observed within a larger population disappears or reverses directions within the sub groups.  A classic example is the Berkley Admissions gender bias study.

Below we'll synthesize some of these paradoxical relationships and plot them.

# Week 4: Matplotlib

## Ticks

Major and minor tick marks on each axis
interior or exterior to axes
alpha allows a degree of transparency
can conver the entire chart

## Canvas

the display is a canvas

## Datetime Objects and More Stacked Bar Charts


# Week 5: Visualization with Seaborn

seaborn needs matplotlib and numpy, pandas
has built-in datasets, and color palettes

## Setting up seaborn

import seaborn as sns

sns.set()
sns.set_style("whitegrid")
sns.lmplot() # a linear regression with the plot

