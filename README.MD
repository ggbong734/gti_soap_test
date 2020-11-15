# GTI Soap Test project 

Project completed under the Operations Technology Development branch of [Gas Technology Institute](hhttps://www.gti.energy/). The title of the project is "Methodology to Estimate Flow Rate of Above Ground Leaks Using a Soap Test". A public version of the project report has been published. 

<p align="center"><img src="images/gti_logo.jpg" height= "85"/></p>

### Objective 

The objective of the project is to develop a method based on soap test to quickly estimate the flow rate of a natural gas leak on an aboveground component at low pressure (<60 psig). One such component could be natural gas meter sets often located in front of residential buildings.

<p align="center"><img src="images/gas_meter.jpg" height= "200"/></p>

### Background

Soap test has been used by gas utilities to grade leaks on aboveground facilities. Characteristics of bubbles produced during soap test is used as the basis for distinguishing between hazardous and non-hazardous leaks.

<p align="center">
  <img src="images/soap_test.jpg" height="220" />
  <img src="images/soap_bubble.jpg" height ="180" /> 
</p>

<p align="center"><img src="images/leak_classification.png" height= "150"/></p>

### Metric for classifying soap test

Metric to characterize soap test results have to be simple enough to be used in the field. Some possible metrics include:
1. Bubble size
2. Bubble formation rate
3. Duration before bubble burst
4. Total volume of bubbles

Only bubble size was deemed to be practical as it was relatively simple to keep track of the largest bubble rather than attempting to estimate average size or measure duration using a stopwatch. Thus, bubble size was selected as the metric for characterizing soap test results in the proposed approach.

### Lab testing

Variables used in lab test are:

<p align="center"><img src="images/lab_variables.jpg" height= "115"/></p>

Leak flow rate was the primary independent variable. We also wanted to determine impact of different soap solutions on bubble characteristics.

Here is the experimental setup for our lab testing:

<p align="center"><img src="images/setup.jpg" height= "270"/></p>

### Lab test results

Key takeaway from lab testing is that there is a progressive change in bubble behavior as leak flow rate increases. There are 4 distinct phases (i.e. foams, small bubbles, large bubbles, soap solution blown off) which can be used to categorize bubble behavior. 

<p align="center"><img src="images/lab_takeaway.jpg" height= "285"/></p>

Soap solution did not affect bubble behavior drastically (chart not shown).

### Field trial

A field trial was performed with a host utility company. A total of 47 residential meter set leaks were visited and each one was tested with the soap test method. The actual leak flow rates of the leaks were also measured for verification purposes. 4 categories were used to classify the results. Based on the bubble characteristics, a category was assigned to each leak.

<p align="center"><img src="images/soap_test_categories.png" height= "190"/></p>

And a tree diagram was used to aid in classifying the results: 

<p align="center"><img src="images/tree_diagram.png" height= "340"/></p>

And representative flow rate (emission factor) for each category can be derived using population leak rate distribution simulated using historical regional data. The values of the emission factors are depicted by the green dots on the horizontal axis.

<p align="center"><img src="images/distribution_results.png" height= "340"/></p>

### Field trial results

The distribution of leak rates measured during the field trial followed a long tail distribution and is consistent with findings from other studies:

<p align="center"><img src="images/distribution.png" height= "260"/></p>

We can then plot the measured leak rate versus categories assigned in the field based on the soap test results. In the scatter plot below, points (individual leaks) in the blue boxes mean that they are correctly assigned where as points below or above the boxes are underestimated/overestimated. 

<p align="center"><img src="images/scatter_plot.png" height= "310"/></p>

A box plot can be plotted to check how well separated the categories are. Ideally we want good distinction between categories which would allow us to better distinguish small versus large leaks. 

<p align="center"><img src="images/box_plot.png" height= "300"/></p>

We can change the 4 categories into 3 by combining the middle two categories (B and C) together. Doing so, will help improve the separation between categories:

<p align="center"><img src="images/box_plot_3cat.png" height= "300"/></p>

Additionally, we can compare how the estimated leak rates (emission factors) match with actual leak rate:

<p align="center"><img src="images/barchart.jpg" height= "240"/></p>

On a side note, we observed a peculiar phenomenon: in some cases, leaks did not produce bubbles even though we could detect natural gas emissions with methane sensors. We initially hypothesized that these leaks were too small to produce bubbles. However, upon plotting the cumulative distribution of leak rates we found that these "no-bubbles" leaks were NOT the smallest in flow rates. There had to be other factors preventing bubble formation. We will explore this further in future phases. 

<p align="center"><img src="images/distribution_no_bubbles.png" height= "300"/></p>

### Method to reduce uncertainty 

We noticed that there could be sources of uncertainty and to minimize uncertainty we can apply a probabilistic method to update the emission factors using fresh new field data. First we analyze the extent of uncertainty in the data using the table below:

<p align="center"><img src="images/uncertainty_table.png" height= "390"/></p>

Then based on the true positive and false positive rate for each category, we can correct the emission factor for that group using this formula:

![Formula](images/formula.jpg)

### Steps to develop company-specific leak classification criteria

A utility company interested in implementing the proposed soap test method can employ a 4-step approach to develop their company-specific categories and associated emission factors for characterizing soap test results:

<p align="center"><img src="images/4step.jpg" height= "300"/></p>

### Credits
The study and report were completed by Gerry Bong, Jarrod Bullen, and Chris Moore. 