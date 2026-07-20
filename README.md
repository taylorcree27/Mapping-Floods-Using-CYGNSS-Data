# Repurposing CYGNSS Reflectivity Data for Rapid Flood Monitoring
<img align = "left" src="https://science.nasa.gov/wp-content/uploads/2023/11/sarp-patch.jpeg?w=1280&format=webp" alt="drawing" width="200"/>Hi there! This summer, I was an intern for NASA's [Student Airborne Research Program (SARP)](https://science.nasa.gov/earth-science/early-career-opportunities/student-airborne-research-program/). After an incredible two weeks of contriubting to flight and field campaigns in Houston, Texas, I spent a few weeks investigating the potential of repurposed CYGNSS data to detect the evolution of evebt-based floods. I want to thank everyone who made this experience possible, but I would particualry like to thank Alex Saunders (SARP West 2026 Coding Mentor) for playing such a critical role in the development of my project and corresponding code. 


## Abstract
The remote sensing of storm-induced flooding events at a meaningful scale remains
challenging due to conflicting spatial and temporal trade-offs among satellites currently in orbit.
Since flood extent prediction models rely on remote sensing data for improvement and
validation, it is important to investigate how remote observations of flooding can be improved.
This research investigates current methodology for repurposing Cyclone Global Navigation
Satellite System (CYGNSS) derived data products to map flooding beneath clouds and
vegetation. CYGNSS has the potential to offer a much higher temporal resolution than is
achievable with traditional, conventionally reliable satellite data sources such as Sentinel-1 and
Sentinel-2 due to their lower revisit frequency and inability to penetrate cloud/vegetation cover,
respectively. Here, the UC Berkeley Level 3 CYGNSS watermask product, created using the
RWAWC (Random Walk Algorithm WaterMask from CYGNSS) segmentation method for pixel
classification, was used to produce maps of flooding caused by Hurricane Ida in New Orleans in
2021. Remotely sensed patterns in flooding captured by CYGNSS are compared against (1)
ground truth flood extent confirmed by in-situ USGS gauges to assess agreement in timing of
water level fluctuation, (2) flood maps derived from Sentinel-1 imagery, to assess the accuracy
of the RWAWC mask data in representing changes in inundation, and 3) narrowed and
repeated analysis for several different land covers (including agricultural, swamp, marsh, and
residential) within the entire area of interest. A confusion matrix comparing Sentinel 1 flood
identification to RWAWC indicated that the model was not successful for this application (CSI=
0.35, FAR: 68.4%, Accuracy: 46.1%). Considering the metrics produced, CYGNSS derived
gridded watermask products may not currently be suited for post-disaster flood monitoring, as
this process requires a very fine spatial resolution and frequent, accurate data updates. The
case study suggests the need for further research to assess the reliability of CYGNSS-derived
flood maps for post-disaster flood monitoring, particularly regarding the classification processes
necessary to produce gridded products for mapping, which may affect the accuracy of the
mapped flood extent. With further development of classification methodology, CYGNSS’s high
revisit time could allow for post-disaster hydrologic dynamics, particularly in coastal
areas/wetlands, to be monitored more extensively than is possible at present.

## About this template

This template was generated as an example for how to format and upload project code to github. Remember that uploading your code can be an interative process - it doesn't have to be perfect the first time! First focus on getting your code online, then move onto progressively organizing the code. Once you reach the cleaning stage some things to look for include:

- Make sure each chunk of code has a comment or markdown explanation of what is happening in the code
- Delete code that isn't ever used. It can be hard (emotionally), but it helps the code you are using be more useful.
- Break your project code into a few different notebooks by analysis step and name them starting with a number. For example: `01_preprocessing.ipynb`, `02_timeseries_analysis.ipynb` and `03_visualization.ipynb`.
- Keep seperate folders for code and figures

To get even deeper into code cleaning, check out the [Good Research Code Handbook](https://goodresearch.dev/index.html).

Some notes:
- If you are using satellite images as part of your analysis they may be too large to upload to github. In that case simply upload your code.
