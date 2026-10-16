# HPLC Vial and Cap Detection Dataset

This dataset contains 65 images with 542 annotated instances of high-performance liquid chromatography (HPLC) vials and caps. 
Annotations are provided in COCO format and contain **bounding boxes only**; segmentation masks are not included.

The dataset is intended for fine-tuning pretrained object detection models, such as Faster R-CNN, to detect vials and caps. 
Its small size should be considered when training models and evaluating their ability to generalize.

## File structure

```text
.
├── images/       # Dataset images
├── result.json   # COCO bounding box annotations
└── README.md
```

Images are stored in the `images/` folder. The `result.json` file contains the image metadata, object categories, and bounding box annotations.

## Annotations

The dataset contains two classes:

- **Cap**
- **Vial**

Each object is annotated with a bounding box. In COCO format, bounding boxes are represented as `[x, y, width, height]` in pixels, where `(x, y)` is the top-left corner of the box.

## Dataset statistics

| Metric | Count |
|---|---:|
| Images | 65 |
| Annotated objects | 542 |
| Caps | 336 |
| Vials | 206 |

### Objects per image

| Objects | Images |
|---|---:|
| 1 | 4 |
| 2 | 4 |
| 3 | 3 |
| 4 | 7 |
| 5 | 3 |
| 6 | 17 |
| 7 | 6 |
| 8 | 3 |
| 11 | 1 |
| 12 | 9 |
| 17 | 1 |
| 18 | 2 |
| 20 | 2 |
| 24 | 1 |
| 37 | 2 |
