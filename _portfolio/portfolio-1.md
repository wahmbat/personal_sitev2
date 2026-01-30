---
title: "Undergraduate Research Assistant (2025–Present) <br> McGuire Center for Lepidoptera and Biodiversity"
collection: portfolio
excerpt: ' '

---

<br>

My research at the McGuire Center, 
performed as part of UF's Emerging Scholars Program and under the guidance of Dr. Keith
Willmott, focuses on the creation and analysis 
of species distribution maps for Neotropical butterflies in the subtribe Euptychiina.
Part of the challenge of this research is in the incomplete and oftentimes 
erroneous nature of entomological specimen data. To address this, and make it easier
for future researchers seeking to create distribution maps, I am working to develop transparent 
and reproducible workflows in R and QGIS for cleaning, validating, and
mapping locality data. The locality data we are utilizing is sourced from a wide variety of places, but mostly come from the Florida Natural History Museum's collections and records from iNaturalist. 

<br>

<div style="display: flex; gap: 20px; flex-wrap: wrap; align-items: flex-start;">
  <img src="{{ '/images/range.png' | relative_url }}" 
       alt="butterfly range" 
       width="300">
  <img src="{{ '/images/map.png' | relative_url }}" 
       alt="butterfly map" 
       width="300">
</div>

<br>

The images above give a glimpse into the workflow we are developing; the species pictured is <i>Amphidecta clio</i>. The image on the left shows the first step in the process: after the locality points are edited and verified for accuracy) an R script draws a buffered polygon encompassing every points. This approach reflects the idea that the species’ range is more uncertain where points are sparse, while in areas with many observations we are more confident that its range does not extend much further. This dynamic approach is a significant improvement from prior mapping techniques, which would often draw a polygon with a constant buffer distance and not account for relative point dispersion. 

The image on the right shows a presence-absence map for <i>Amphidecta clio</i> (white indicating areas that lie in their predicted range and black indicating areas that do not). These maps were produced using the Wallace EcoMod package in R, which identifies the map cells within the previously drawn polygon that fall within the species’ plausible climatic range, based on the locality data.
    
Following the creation of these distribution maps, Dr. Willmott and I plan to conduct statistical analysis
on the emerging patterns in Euptychian species diversity across the Neotropics, specifically in 
relation to the ecological hypothesis of the mid-domain effect (MDE). The MDE is a proposed null
model in macroecology which suggests that species richness will peak in the center of a bounded 
geographical region due to the natural random overlap of species ranges. We plan to investigate this 
phenomenon by analyzing the degree to which geographic factors, namely the distance from the nearest continental 
boundary, predicts Euptychian species richness while controlling for other biological and environmental variables.








