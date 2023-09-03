# Leaf-Segmentation-Classification
Segmenting leaf images and categorizing them into one of 38 classes, distinguishing between diseased and healthy leaves.

# Plant Diseases Classification
The project aims to build a model that can be used to classify plant images into their respective class.

* The dataset ([plantvillage-dataset](https://github.com/spMohanty/PlantVillage-Dataset)): has 38 different classes of healthy and diseased plants

* We will use three pre-trained models to evaluate and choose the one that has the best perfomance, the models are:
    * [Resnet34](https://arxiv.org/pdf/1512.03385.pdf)
    * [VGG16](https://arxiv.org/pdf/1409.1556.pdf)    
    * [Densenet169](https://arxiv.org/pdf/1608.06993.pdf)
    
* We will employ two different loss functions to evaluate the one with the best performance in-order to tackle the problem of class-imbalanc. the loss functions are:
    * [Cross Entropy Loss](https://machinelearningmastery.com/cross-entropy-for-machine-learning/)
    * [Focal Loss](https://paperswithcode.com/method/focal-loss)
 
# Leaf Segmentation & Classification
The project's objective is to develop a model capable of both segmenting leaf images and categorizing them into one of 38 classes, distinguishing between diseased and healthy leaves.



*  The dataset utilized in this project is the [PlantVillage-Dataset](https://github.com/spMohanty/PlantVillage-Dataset) containing images of leaves, corresponding masks, and spanning across 38 distinct classes.

*   Our methodology comprises two primary phases:

      1.  Creating [COCO-annotations](https://cocodataset.org/#home) in order to train a Mask R-CNN model using [Detectron2](https://github.com/facebookresearch/detectron2). Since the dataset contains masks in image format, we need to convert them into the COCO format.

      2.   Train the Detectron2 model using the COCO-annotations JSON file generated and the provided dataset.






