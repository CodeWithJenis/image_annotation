# Football Semantic Segmentation Dataset (COCO 1.0)

## Project Overview
This dataset is specifically designed for semantic segmentation tasks in football-related scenarios. It includes pixel-level annotations to identify and segment objects like players, ball, and other football-related elements in the images. The dataset is stored in COCO format, making it suitable for advanced segmentation models.

## Annotation Details
- **Annotation Types:** 
  - Semantic Segmentation
- **Annotation Format:** COCO JSON
- **Labels:** Football-related objects (e.g., players, ball, ground, etc.)

## Tools Used
- **Annotation Tool:** CVAT (Computer Vision Annotation Tool)

## How to Use
1. Load the images and annotations into frameworks supporting COCO format (e.g., Detectron2, Mask R-CNN).
2. Use the `annotations/` folder for training, validation, and testing.
3. Ensure the `images/` folder contains the corresponding original images.

## Challenges
- **Semantic Segmentation:** Achieving pixel-perfect masks for objects like players,ball,audience and so on was challenging due to occlusions and varying lighting conditions.
- **Consistency:** Maintaining consistent labeling for objects across multiple images was crucial for ensuring the quality of the dataset.

## Dataset Structure
The dataset is organized as follows:

```
/football_semantic_segmentation_coco1.0/
├── annotations/                
│   ├── instances_default.json  # COCO JSON file for semantic segmentation annotations
├── images/                     
│   ├── default                 # Folder containing original football images
├── README.md                   # Description of the dataset and the annotation process
├── football_semantic_segmentation_coco1.0.mp4 # Video explanation of the annotation project
```

---
