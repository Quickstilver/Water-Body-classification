# Water-Body-classification

Glint Solar: Accelerating Renewable Energy Adoption with AI-Powered Water Body Classification

## Project Description

Glint Solar is dedicated to driving the adoption of renewable energy by streamlining the planning and development phase while improving outcomes and reducing costs. Our software enables swift screening and evaluation of potential sites for ground-mounted and floating solar installations.

This project focuses on a critical aspect of floating solar installations: identifying artificial water bodies. Solar developers often prefer to build on artificial water bodies (e.g. hydro-power reservoirs, water treatment plants) as they typically have an easier time obtaining permission. To help our customers find these artificial water bodies, we developed a machine learning model capable of classifying any given water body as artificial or natural.

## Data and Implementation

We worked with two datasets, Water Bodies in Rhode Island and the National Inventory of Dams, to identify and visualize artificial water bodies in Rhode Island. Using a Jupyter Notebook, we created a script that leverages GeoPandas, Shapely, and other libraries to process and visualize geospatial data.

To identify artificial water bodies, we used a shape-based approach. We calculated the rectangularity of each water body and considered it artificial if its area was more than 85% (perfect circle would have pi/4 about 78% overlap), of the area of its minimum bounding rectangle. After identifying artificial water bodies, we downloaded cropped Sentinel-2 images for the three largest and three smallest water bodies in Rhode Island.

## Challenges and Potential Solutions

There are several challenges when working with shape-based approaches for artificial lake identification, such as false positives and difficulties in data availability. To address these issues, we proposed alternative solutions such as supervised classification, clustering, and incorporating additional features. By continuously integrating diverse data sources and leveraging supervised classification systems, we can enhance data and progressively improve accuracy.

## Libraries Used

- GeoPandas
- Shapely
- Rasterio
- Rioxarray
- Sat-search
- Matplotlib

## Conclusion

This project showcases our commitment to harnessing the power of data science and artificial intelligence to accelerate renewable energy adoption. By identifying artificial water bodies, we empower solar developers with the information they need to make informed decisions and contribute to a more sustainable future.
