The following notebook should run from start to end without errors. If not, please open an issue.
Consider running with Google Colab for a swift run-through.

# In this repository I:
## multi-label classification
  - analyze and preprocess the PASCAL VOC 2009 dataset
  - try solve data imbalance issues, define loss function, and determine metrics 
  - build two CNN multi-label classifiers based on existing architectures in Keras
        - one based on a simplified more shallow version of VGG with 2 versions (one with globalaveragepooling layer and one without)
        - one based on Resnet50v2 (only for demonstration)
  - train two version the VGG classifier with data augmentation enabled
  - plot overal performance and class based performance
  - use Class Activation Maps to debug the trained CNN
  - propose solutions for the class imbalance problem
  - use Transfer Learning to achieve better performance
        - solution is a pretrained MobileNet CNN on ImageNet
  - plot performance after Transfer Learning and present improvements
## break the classifier
  - train a binary image classifier (with transfer learning)
  - build an adverserial network (Autoencoder) to generate perturbations
  - add perturbations to original image to break the binary image classifier
  - increase perturbations and verify tradeoff
  
# Dataset and pretrained models

- In this notebook a slightly restructured version of the PASCAL VOC 2009 dataset is used. It will be automatically fetched from Google Drive.
- All models used in this notebook are automatically fetched. If you want to train them from scratch, change the booleans accordingly .
- If you are unable to fetch dataset or the models, please open an issue of contact the author. 

# Disclaimer

The author is not responsible nor accountable for the utilization of this code in any given setting. Please do not use this in production. 
