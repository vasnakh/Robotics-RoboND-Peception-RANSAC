# Tabletop Segmentation
![screen shot 2017-07-05 at 10 49 11 am](https://user-images.githubusercontent.com/20687560/27878614-aff58b20-6173-11e7-909d-41d5d21a23d6.png)
This code applies some filtering techniques and use RANSAC plane fitting to segment the table in point cloud.  

### Note: This exercise requires Python 2 due to the Python bindings to PCL being used here.  If you installed Python via Anaconda using the RoboND-Python-Starterkit, you have Python 3 installed in your RoboND conda environment so this exercise won't work.  




In brief, the steps are the following:

1. Downsample the point cloud by applying a Voxel Grid Filter.
2. Apply a Pass Through Filter to isolate the table and objects.
3. Perform RANSAC plane fitting to identify the table.
4. Use the ExtractIndices Filter to create new point clouds containing the table and objects separately.

### To view a .pcd file:

```
$ pcl_viewer filename.pcd 
```
