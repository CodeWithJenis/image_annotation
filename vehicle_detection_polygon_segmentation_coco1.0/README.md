# Vehicle Detection Dataset (Polygon Segmentation - COCO 1.0)

## Project Overview
This dataset is designed for vehicle detection tasks, using polygon segmentation annotations to capture the precise shapes of vehicles in each image. The dataset is saved in COCO format, making it suitable for instance segmentation and other computer vision tasks that require detailed object boundaries.

## Annotation Details
- **Annotation Type:** Polygon segmentation
- **Annotation Format:** COCO JSON
- **Labels:** Vehicles (e.g., cars, ambulances, buses,motercycle etc)

## Tools Used
- **Annotation Tool:** CVAT (Computer Vision Annotation Tool)

## How to Use
1. Load the images and annotations into frameworks supporting the COCO format (e.g., Detectron2, Mask R-CNN).
2. Use the `annotations/` folder for training, validation, and testing.
3. Ensure the `images/` folder contains the corresponding images referenced in the COCO JSON file.

## Challenges
- **Complex Shapes:** Annotating polygons for vehicles with irregular shapes (e.g., motercycle and ambulances(half image part only))  was challenging.
- **Consistency:** Ensuring the polygons closely follow the vehicle's edges while maintaining consistency across all images.

## Dataset Structure
The dataset is organized into the following structure:

```
/vehicle_detection_polygon_segmentation_coco1.0/
├── annotations/               # Folder containing polygon segmentation annotations (COCO JSON format)
│   ├── instances_default.json # COCO JSON file for training annotations
├── images/                    # Folder containing original vehicle images 
│   ├── image1.jpg             # Example image file
│   ├── image2.jpg
│   └── ...
├── README.md                  # Description of the dataset and the annotation process
├── vehicle_detection_polygon_segmentation_coco1.0.mp4 # Video explaination of the whole project
```
