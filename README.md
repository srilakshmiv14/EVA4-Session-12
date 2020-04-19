# EVA4-Session-12

Assignment A:
1.	Download this TINY IMAGENET (http://cs231n.stanford.edu/tiny-imagenet-200.zip)dataset. 
2.	Train ResNet18 on this dataset (70/30 split) for 50 Epochs. Target 50%+ Validation Accuracy. 
3.	Submit Results. Of course, you are using your own package for everything.

Part A Assignment
1.	Importing all the packages.
2.	Modules are stored in a library which is available in Session 8 repository folder named Library - https://github.com/srilakshmiv14/EVA4-Session-8-Library

For Session 12 the new modules are Tinyimagenet dataset(representation of classes)
Modules are 
1.	Installing Albumentation package and Library link to modules
2.	Importing necessary modules from library to run the code.
3.	Train and Test Transforms 
4.	Load and Split Datasets
5.	Taking model from Torchvision ResNet18 and setting Number of classes to 200
6.	Printing the model Summary
7.	Training and Testing Using SGD Optimizer and OnecycleLR Scheduler 
8.	Plot Train and Test Accuracy
9.	Plot Gradcam of 10 Misclassified Images

Modules Description:
I. Loading TinyImageNet Datasets.
II. Transformations done: Albumentations :
1.	Rotate,
2.	Adding PadIfneeded(70),
3.	Horizontal flip,
4.	RandomCrop(64),
5.	RGB Shift, Normalize,
6.	Cutout strategy 
III. Loading and running Train dataset and Test dataset:
We have used SGD Optimizer with learning rate 0.01 and Momentum 0.9 and included One Cycle LR Scheduler
Model Parameters are 11,271,232
Ran the model with 50 epochs with batch size 256
Train set: Average loss:  0.0012      Accuracy: 92.06%
Test set: Average loss:  1.7864        Accuracy: 62.35%
Final Accuracy of the model is 62.35 %


Assignment B:
1.	Download 50 images of dogs. 
2.	Use this (http://www.robots.ox.ac.uk/~vgg/software/via/via_demo.html) to annotate bounding boxes around the dogs.
3.	Download JSON file. 
4.	Describe the contents of this JSON file in FULL details (you don't need to describe all 10 instances, anyone would work). 
5.	Refer to this tutorial (https://towardsdatascience.com/machine-learning-algorithms-part-9-k-means-example-in-python-f2ad05ed5203). Find out the best total numbers of clusters. Upload link to your Colab File uploaded to GitHub. 
