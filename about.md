---
layout: page
title: About
permalink: /about/
---

{{ site.description }}

The risk rating scale is based on the [COVID Risk Levels Dashboard from Harvard Global Health Institute](https://globalepidemics.org/key-metrics-for-covid-suppression/), which was released on July 1, 2020. Please see that site for more information on the rating scale.

I made this site for a few reasons:

1. I wanted to see how the risk levels changed over time, and the Harvard site does not provide historical risk ratings.
2. The Harvard site can move very slow if the site gets lots of traffic. I built this in such a way that the site should never slow down as a result of traffic spikes.
3. Since I live in Texas, the Texas data is most important to me.
4. The case data used on the Harvard site seems to be lagging 24 hours behind data from Texas Health and Human Services.
5. While the 4-color rating is helpful and simple, the risk between a 7DMA of 24 and 25 is much closer than the risk between 10 and 24. So, I also wanted to create a map that has a gradual color scale that reflected the increasing risk level as the 7DMA changes. I provide both maps: First the map using the Harvard rating scale, and then a second map using a gradual color scale. The Harvard rating scale is:
  - Green: 7-Day moving averages (7DMA) less than 1
  - Yellow: 7DMA between 1-9
  - Orange: 7DMA between 10-24
  - Red: 7DMA greater than 25



### Methodology

I calculate daily case data using information from [Texas Health and Human Services](https://txdshs.maps.arcgis.com/apps/opsdashboard/index.html#/ed483ecd702b4298ab01e8b9cafc8b83) (click on the "Additional Data" tab and see "Cases over Time by County"). Then, I take the average of the most recent 7 days to get the moving average, and generate the number of cases per 100,000. There is some discrepancy between my 7-day moving average and the one provided by Harvard. My guess is that they are using different population estimates. I use the county population data provided in the Excel file from Texas Health and Human Services.

The site is built using [Jekyll](https://jekyllrb.com/) and [FusionCharts](https://www.fusioncharts.com/).

### About Me

My name is Matt Cleaver, and I enjoy dabbling in random projects. I'm not a professional coder, web developer, or epidemiologist. I teach philosophy at Trinity Valley Community College. None of the information presented here is guaranteed to be accurate, so proceed accordingly.
