# Bio-Physical-Parameters-of-Tree
This repo contains the infromation about various biophysiological parameters of a tree 

# Bio-physical parameters of a tree

**1. Vapour-pressure deficit, or VPD**

It is the difference (deficit) between the amount of moisture in the air and how much moisture the air can hold when it is saturated. Once air becomes saturated, water will condense out to form clouds, dew or films of water over leaves. It is this last instance that makes VPD important for greenhouse regulation. If a film of water forms on a plant leaf, it becomes far more susceptible to rot. On the other hand, as the VPD increases, the plant needs to draw more water from its roots. In the case of cuttings, the plant may dry out and die. For this reason the ideal range for VPD in a greenhouse is from **0.45 kPa to 1.25 kPa**, ideally sitting at around 0.85 kPa. As a general rule, most plants grow well at VPDs of between 0.8 and 0.95 kPa.

To compute the VPD, we need the ambient (greenhouse) air temperature, the relative humidity and, if possible, the canopy air temperature. We must then compute the saturation pressure. Saturation pressure can be looked up in a psychrometric chart or derived from the Arrhenius equation. 

Formulation: https://en.wikipedia.org/wiki/Vapour-pressure_deficit

Basics of VPD: https://pulsegrow.com/blogs/learn/vpd


**2. Arrhenius equation**

In physical chemistry, the Arrhenius equation is a formula for the temperature dependence of reaction rates. The equation was proposed by Svante Arrhenius in 1889, based on the work of Dutch chemist Jacobus Henricus van 't Hoff who had noted in 1884 that the van 't Hoff equation for the temperature dependence of equilibrium constants suggests such a formula for the rates of both forward and reverse reactions. This equation has a vast and important application in determining the rate of chemical reactions and for calculation of energy of activation. Arrhenius provided a physical justification and interpretation for the formula.[1][2][3][4] Currently, it is best seen as an empirical relationship.[5]: 188  It can be used to model the temperature variation of diffusion coefficients, population of crystal vacancies, creep rates, and many other thermally-induced processes/reactions. The Eyring equation, developed in 1935, also expresses the relationship between rate and energy.

Formulation: https://en.wikipedia.org/wiki/Arrhenius_equation


**3. Potential Evapotranspiration (PET)**



**4. Leaf Surface Resistance**


Reference: https://escomp.github.io/ctsm-docs/versions/master/html/tech_note/Photosynthesis/CLM50_Tech_Note_Photosynthesis.html


**5. Canopy Surface Temperature**



**6. Leaf Capacitance**



**7. Leaf Area Index**


**8. Leaf Temperature**

*  Normalized Relative Conopy Temperature (NCRT) = (Tcanopy - Tmin) / (Tmax - Tmin)


**9. Chlorophyll Fluorescence**



**10. Leaf Spectrometry**

**11. Leaf Water Content**

**12 Light Extinction Coefficient**


Reference: https://link.springer.com/article/10.1007/s13580-011-0216-3

**13. Spectral Indices**

[https://github.com/ParthaPRay/AS7265x-Spectral-Indices](url)

* NDVI = (NIR - Red)/(NIR + Red)

* CNDVI = (NIR<sub>940</sub> - Red<sub>660</sub>)/(NIR<sub>940</sub> + Red<sub>660</sub>)

* WDVI = NIR - slope_soil * Red;
  
* PVI = (NIR - slope_soil × Red - intercept) / sqrt(slope_soil^2 + 1)
  
*  DVI = NIR - Red
  
*  TNDVI = sqrt((NIR - Red) / (NIR + Red) + 0.5)
  
*  EVI = 2.5 × ((NIR - Red) / (NIR + 6 × Red - 7.5 × Blue + 1))
  
*  SAVI = (1 + slope_soil) × (NIR - Red) / (NIR + Red + slope_soil)
  
*  GNDVI = (NIR - Green) / (NIR + Green)
  
*  TVI = 0.5 * (120 * (NIR - Green) - 200 * (Red - Green))
  
*  VARI = (Green - Red) / (Green + Red - Blue)
  
*  ExG = 2*Green - Red - Blue
  
*  ExR = 1.4*Red - Green
  
*  ExB = 1.4*Blue - Green
  
*  NGRDI = (Green - Red) / (Green + Red)
  
*  CIVE = 0.441Red - 0.811Green + 0.385*Blue + 18.78745
  
*  GLI = 2*Green - Red - Blue
  
*  CI = (NIR / Red) - 1
  
*  GCI = (NIR/Green) − 1
  
*  DGCI = (NIR - Green) / (NIR + Green)
  
*  PRI = (R531 - R570) / (R531 + R570)
  
*  RVI = NIR/Red
  
*  MNLI = (1 - 0.5) * ((1.08*(NIR-Red))/(1 + sqrt(NIR-Red)))
  
*  TCARI = 3 * ((Green-Red) - 0.2 * (Green-Blue) * (Green/Red))
  
*  MCARI = ((Red - Green) - 0.2 * (Red - Blue)) * (Red/Green)
  
*  RECI = (NIR/Red_edge) - 1
  
*  MSRI = ((NIR/Red) - 1) / (NIR/Blue)

* ARVI = (NIR - Red)/ (NIR + Red - 2* Blue)

* MSAVI = (1/2)* [2*(NIR+1) - Sqrt( (2*NIR+1)^2 - 8*(NIR -Red) )]

* Meris Terrestrial Chlorophyll Index  (MTCI) = (NIR -Red)/(Red- Blue)

* Normalized Difference Red-Edge Index (NDRE) = (NIR - RedEdge)/ (NIR + RedEdge)

* RENDVI = (NIR<sub>940</sub> - R<sub>710</sub>)/(NIR<sub>940</sub> + R<sub>710</sub>)     



**Follwoing are difficult to measure by using AS7265x**



* OSAVI = (1.16 * (NIR<sub>840</sub> - R<sub>660</sub>)/(NIR<sub>840</sub> + R<sub>640</sub> + 0.16)     _...AS7265x NOT Possible_
* RDVI = (NIR<sub>840</sub> - R<sub>660</sub>)/(NIR<sub>840</sub> + R<sub>660</sub>)*(1/2)      _...AS7265x NOT Possible_
* SIPI = (NIR<sub>840</sub> - B<sub>450</sub>)/(NIR<sub>940</sub> + R<sub>660</sub>)    _...AS7265x NOT Possible_
* Anthocynanin Reflectance Index (ARI) = 1/R<sub>550</sub>) - 1/R<sub>700</sub>)     _...AS7265x NOT Possible_ 
* Caretenoid Reflectance Index (CRI) = 1/R<sub>510</sub>) - 1/R<sub>550</sub>)    _...AS7265x NOT Possible_
* Water Band Index (WBI) = R<sub>970</sub>)/R<sub>900</sub>)         _...AS7265x NOT Possible_


# GLCM

*  Grey Level Co-occurance Matrix (GLCM) contains Mean, Variance, Homogeneity, Contrast, Dissimilarity, Entropy, Second Moment, Correlation


# Various Parameters

* Various paramters of climate change:  Read Brun, P., Zimmermann, N.E., Hari, C., Pellissier, L., Karger, D.N. (preprint): Global climate-related predictors at kilometre resolution for the past and future. Earth Syst. Sci.     Data Discuss. https://doi.org/10.5194/essd-2022-212


# Calibration 

**1. Multivarite Claibration Techniques**

  * Partial least squares (PLS)
  * Support vector regression (SVR)
  * Least squares support vector machine regression (LSSVR)
  * Radial basis function (RBF) neural network (NN)

# Error Detection and Analysis

* PCA

* Standard error of calibration (SEC)
* Standard error of prediction (SEP)
* Bias
* R<sup>2</sup>
* MSE
* RMSE
* MAPE
* RPD
  

