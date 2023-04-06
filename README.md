# Water-Body-classification

## Project Description

This project focuses on a critical aspect of floating solar installations: identifying artificial water bodies. Solar developers often prefer to build on artificial water bodies (e.g. hydro-power reservoirs, water treatment plants) as they typically have an easier time obtaining permission. To help find these artificial water bodies, I developed a machine learning model capable of classifying any given water body as artificial or natural.

## Libraries Used

- GeoPandas
- Shapely
- Rasterio
- Rioxarray
- Sat-search
- Matplotlib

## Data and Implementation

I mainly owrked with two  datasets, Water Bodies in Rhode Island and Sentinel-2 Data, to identify and visualize artificial water bodies in Rhode Island. Using a Jupyter Notebook, I created a script that leverages GeoPandas, Shapely, and other libraries to process and visualize geospatial data.

To identify artificial water bodies, I designed an innovative a shape-based approach. I calculated the rectangularity of each water body and considered it artificial if its area was more than 85% (perfect circle would have pi/4 about 78% overlap), of the area of its minimum bounding rectangle. After identifying artificial water bodies, I downloaded cropped Sentinel-2 images for the three largest and three smallest water bodies in Rhode Island.

## Open challenges and Potential Solutions

There are several challenges when working with shape-based approaches for artificial lake identification, such as false positives and difficulties in data availability. To address these issues, I proposed alternative solutions such as supervised classification, clustering, and incorporating additional features. By continuously integrating diverse data sources and leveraging supervised classification systems, I can enhance data and progressively improve accuracy.


## Conclusion

This project showcases my commitment to harnessing the power of data science and artificial intelligence to accelerate renewable energy adoption. By identifying artificial water bodies, I empower solar developers with the information they need to make informed decisions and contribute to a more sustainable future.
