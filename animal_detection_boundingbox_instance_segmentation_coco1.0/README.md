# Animal Detection Dataset (Bounding Box & Instance Segmentation - COCO 1.0)

## Project Overview
This dataset is designed for animal detection tasks, using both bounding box and instance segmentation annotations. It includes a variety of animal species(rhino,bear,bobcat etc), with precise bounding boxes and segmentation polygons to accurately detect and classify them in different environments. The dataset is stored in COCO format, suitable for both object detection (bounding box) and instance segmentation tasks.

## Annotation Details
- **Annotation Types:** 
  - Bounding Boxes
  - Instance Segmentation
- **Annotation Format:** COCO JSON
- **Labels:** Animals (e.g., antelope,bear,bobcat,chimpanzee,hippopotamus,rhino,other etc.)

## Tools Used
- **Annotation Tool:** CVAT (Computer Vision Annotation Tool)

## How to Use
1. Load the images and annotations into frameworks supporting the COCO format (e.g., Detectron2, Mask R-CNN).
2. Use the `annotations/` folder for training, validation, and testing.
3. Ensure the `images/` folder contains the corresponding images referenced in the COCO JSON file.

## Challenges
- **Bounding Boxes:** Some animal images have a complex background, making it difficult to accurately place bounding boxes.
- **Instance Segmentation:** Creating polygons for animals that are partially obstructed or overlapping with other objects posed a significant challenge.
- **Consistency:** Ensuring the annotations followed the animal's outline accurately while being consistent across multiple images.

## Dataset Structure
The dataset is organized into the following structure:

```
/animal_detection_boundingbox_instance_segmentation_coco1.0/
├── annotations/                # Folder containing bounding box and instance segmentation annotations (COCO JSON format)
│   ├── instances_default.json  # COCO JSON file for bounding box and instance segmentation annotations
├── images/                     
│   ├── default                 #Folder containing original animal images 
│   ├── image1.jpg              # Example animal image file 1
│   ├── image2.jpg
│   └── ...
├── README.md                   # Description of the dataset and the annotation process
├── animal_detection_boundingbox_instance_segmentation_coco1.0.mp4 # Video explaination of the whole project
```

---