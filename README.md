# using_pycocotools

How to use Pycocotools and CocoDataset. Pycocotools detailed explanation.

[https://cocodataset.org](https://cocodataset.org)

---

![people_with_annotations.png](H:\My%20Drive\github\using_pycocotools\images\people_with_annotations.png)

# What is COCO?

![](https://cocodataset.org/images/coco-icons.png)

COCO is a large-scale object detection, segmentation, and captioning dataset. COCO has several features:

- Object segmentation
- Recognition in context
- Superpixel stuff segmentation
- 330K images (>200K labeled)
- 1.5 million object instances
- 80 object categories
- 91 stuff categories
- 5 captions per image
- 250,000 people with keypoints

# COCO Dataset Formats

**Images:** Provides all the image information in the dataset without bounding box or segmentation information. An example of image information

```json
“image”: [{'license': 4,
  'file_name': '000000252219.jpg',
  'coco_url': 'http://images.cocodataset.org/val2017/000000252219.jpg',
  'height': 428,
  'width': 640,
  'date_captured': '2013-11-14 22:32:02',
  'flickr_url': 'http://farm4.staticflickr.com/3446/3232237447_13d84bd0a1_z.jpg',
  'id': 252219 
}]
```

**Annotations:** Provides a list of every individual object annotation from each image in the dataset.

```json
anns [
{'segmentation': [[361.81, …, 365.48]], 
'num_keypoints': 17, 
'area': 8511.1568, 
'iscrowd': 0, 
'keypoints': [356, 198, 2, …, 355, 354, 2], 
'image_id': 252219, 
'bbox': [326.28, 174.56, 71.24, 197.25], 
'category_id': 1, 
'id': 481918}, 
…
]
```

# Sources and Tutorials

- [cocoapi/pycocoDemo.ipynb at master · cocodataset/cocoapi · GitHub](https://github.com/cocodataset/cocoapi/blob/master/PythonAPI/pycocoDemo.ipynb)

- [Introduction to the COCO Dataset - OpenCV](https://opencv.org/introduction-to-the-coco-dataset/)
