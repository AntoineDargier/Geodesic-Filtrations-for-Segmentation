# Geodesic Filtrations for Segmentation
Foundations of Geometric Methods in Data Analysis course, CentraleSupélec x Inria, Spring 2023

### Goal
Use of Topological data analysis (TDA) and mainly persistent homology to compute shape segmentation

### Language
```Python```

### Contents
1. Geodesic distances
2. Point signatures
3. Stability theorem
4. Statistical tests
5. Segmentation models

### Libraries
* ```gudhi```
* ```numpy```
* ```heapq```
* ```scikit-learn```
* ```matplotlib```

### Conclusion
I explored the use of geodesic filtrations for shape segmentation. To do this, I first created geodesic distances on shapes, which measure the shortest path between any two points on the shape’s surface. Next, I used the geodesic distances as filtration to compute persistence diagrams. Persistence diagrams are a way to capture
the topological features of a shape at different spatial scales.  To evaluate the stability of our method, I used the stability theorem, which states that small changes in the shape or the filtration parameter should result in only small changes in the persistence diagrams. I tested the theorem by computing the PDs for similar shapes or close basepoints and comparing the resulting persistence diagrams to the original ones. I designed statistical tests to distinguish between different shapes based on their persistence diagrams. Finally, I have used different methods to vectorise persistence diagrams, and have used them to train machine learning models. With excellent accuracy of 92%, I was able to recognise and classify different parts of a human body, such as arms, legs or head.
