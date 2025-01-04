# Vehicle Detection Dataset (Bounding Box Annotations - Pascal VOC 1.1)

## Project Overview
This dataset is designed for vehicle detection tasks, using bounding box annotations to mark the location of vehicles in each image. The dataset is saved in Pascal VOC format, making it compatible with a variety of object detection frameworks like YOLO and SSD.

## Annotation Details
- **Annotation Type:** Bounding boxes
- **Annotation Format:** Pascal VOC XML
- **Labels:** Vehicles (e.g., cars,ambulances,motercycle,buses etc)

## Tools Used
- **Annotation Tool:** CVAT (Computer Vision Annotation Tool)

## How to Use
1. Load the images and annotations into your preferred object detection framework.
2. Use the `Annotations/` folder for training and testing your model.
3. Refer to `labelmap.txt` for mapping class labels to IDs.

## Challenges
- Maintaining consistent bounding box sizes for various vehicle types.
- Ensuring bounding boxes accurately cover vehicles without including excess background.

## Dataset Structure
The dataset is organized into the following structure:

```

/vehicle_detection_boundingbox_pascal_voc1.1/
├── Annotations/               # Folder containing bounding box annotations (VOC XML format)
│   ├── image1.xml             # Example annotation file
│   ├── image2.xml
│   └── ...
├── ImageSets/                 # Folder containing Main folder
│   ├── Main                   # This is Folder containing default.txt
│   ├── default.txt            # List of all image filenames (or custom split)
├── JPEGImages/                # Folder containing raw vehicle images
│   ├── image1.jpg             # Example image file
│   ├── image2.jpg
│   └── ...
├── labelmap.txt               # Text file mapping class labels to numeric IDs
├── README.md                 # Markdown file providing detailed information of the project
├── vehicle_detection_boundingbox_pascal_voc1.1.mp4   # Video explaination of the whole project

```
