# Forest-Cover-Type-Dataset
- Tree types found in the Roosevelt National Forest in Colorado

## About Dataset
### Context:
This dataset contains tree observations from four areas of the Roosevelt National Forest in Colorado. All observations are cartographic variables (no remote sensing) from 30 meter x 30 meter sections of forest. There are over half a million measurements total!

### Content:
This dataset includes information on tree type, shadow coverage, distance to nearby landmarks (roads etcetera), soil type, and local topography.

### Acknowledgement:
This dataset is part of the UCI Machine Learning Repository, and the original source can be found here. The original database owners are Jock A. Blackard, Dr. Denis J. Dean, and Dr. Charles W. Anderson of the Remote Sensing and GIS Program at Colorado State University.

### Questions to be addressed:

1. Can you build a model that predicts what types of trees grow in an area based on the surrounding characteristics?
2. What kinds of trees are most common in the Roosevelt National Forest?
3. Which tree types can grow in more diverse environments? Are there certain tree types that are sensitive to an environmental factor, such as elevation or soil type?

### Dataset Description
The study area includes four wilderness areas located in the Roosevelt National Forest of northern Colorado. Each observation is a 30m x 30m patch. You are asked to predict an integer classification for the forest cover type. The seven types are:

1 - Spruce/Fir
2 - Lodgepole Pine
3 - Ponderosa Pine
4 - Cottonwood/Willow
5 - Aspen
6 - Douglas-fir
7 - Krummholz

### Aim of the project:
### The training set (15120 observations) contains both features and the Cover_Type. The test set contains only the features. The aim of this project is to predict the Cover_Type for every row in the test set (565892 observations) using Random Forest Classifier, Extra Trees Classifier and Support Vector Machine. Then, my goal is to evaluate which model works the best for the classification.

### Data Dictionary
•Elevation - Elevation in meters
</br>
•Aspect - Aspect in degrees azimuth
</br>
•Slope - Slope in degrees
</br>
•Horizontal_Distance_To_Hydrology - Horz Dist to nearest surface water features
</br>
•Vertical_Distance_To_Hydrology - Vert Dist to nearest surface water features
</br>
•Horizontal_Distance_To_Roadways - Horz Dist to nearest roadway
</br>
•Hillshade_9am (0 to 255 index) - Hillshade index at 9am, summer solstice
</br>
•Hillshade_Noon (0 to 255 index) - Hillshade index at noon, summer solstice
</br>
•Hillshade_3pm (0 to 255 index) - Hillshade index at 3pm, summer solstice
</br>
•Horizontal_Distance_To_Fire_Points - Horz Dist to nearest wildfire ignition points
</br>
•Wilderness_Area (4 binary columns, 0 = absence or 1 = presence) - Wilderness area designation
</br>
•Soil_Type (40 binary columns, 0 = absence or 1 = presence) - Soil Type designation
</br>
•Cover_Type (7 types, integers 1 to 7) - Forest Cover Type designation

### The wilderness areas are:
</br>
1 - Rawah Wilderness Area
</br>
2 - Neota Wilderness Area
</br>
3 - Comanche Peak Wilderness Area
</br>
4 - Cache la Poudre Wilderness Area


### Conclusion:
### •Type 2 (Lodgepole Pine) is the most common type of trees in Roosevelt National Forest

### •Douglas-fir has a normal distribution in terms of aspects, while Cottonwood/Willow has a left-skewed distrubtion, where a significant number of outliers in aspects, ranging from 270-350. 

### •Krummholz tends to grow at a higher height, while Cottonwood/Willow tends to grow at lower height.

### •Ponderosa Pine tends to grow at steeper soil, while Spruce/Fir tends to grow at flatter soil.

### •Overall speaking, Random Forest Classifier does the best job in classifying the tree types, while Support Vector Model works perfectly in disginuishing tree type 5, 6 and 7.
