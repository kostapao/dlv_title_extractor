# dlv_title_extractor
Goal of the project is to extract titles from lecture slides using a pre-build detectron2 model.

## Data

The data consists of lecture slides received during the Master at HSLU Applied information and Data Science.
Following steps were necessary to create the training, validation and test data:

1. Download lecture slides
2. Convert slides to images with [pdf2image](https://pdf2image.readthedocs.io/en/latest/index.html)
3. Annotate images with [makesense.ai](https://www.makesense.ai/)
5. Convert annotations from Pascal VOC XML to COCO format with [voc2coco](https://github.com/yukkyo/voc2coco)

## Model

The model used for training is [detectron2 faster_rcnn_X_101_32x8d_FPN_3x](https://github.com/facebookresearch/detectron2/blob/master/configs/COCO-Detection/faster_rcnn_X_101_32x8d_FPN_3x.yaml)


