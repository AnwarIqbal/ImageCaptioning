# ImageCaptioning

File Descriptions:
1) CleanDescription.ipynb - Data Cleaning
2) Pickle.ipynb - Features Extraction
3) GRUInceptionV3.ipynb - Caption Generating Model

The model focused on generating decription for images with structures in New Zealand. The training dataset contained images available in public domain on social media platforms, captions of which were manually created.

**The Methodology adopted is shown below:**


<image src = "Images/Flow.png">

**Encoder Decoder Merge Model Architecture is adopted as shown below:**


<image src = "Images/Architecture.png">

Feature Extraction of Images: features from the images were preprocessed using with Inception V3, without the output layer, The features thus extracted will act as an input for this model.

Processing of Sequence: This is the Gated Recurrent Unit neural network layer for word embedding pre-trained on GloVe model for text input handling.

Decoder: The output from the above two parts is a vector of fixed length which is merged together to make a final prediction after being processed by a Dense layer.


**Summary of the architecture is shown below:**


<image src = "Images/GRUModel.png">

**Results for some of the captions generated are mentioned below:**


<image src = "Images/Results.png">
  

# References

Jeffrey Pennington, Richard Socher, and Christopher D. Manning. 2014. GloVe: Global Vectors for Word Representation.

Szegedy, C., Vanhoucke, V., Ioffe, S., Shlens, J., & Wojna, Z. (2016). Rethinking the inception architecture for computer vision. In Proceedings of the IEEE conference on computer vision and pattern recognition (pp. 2818-2826).

Tanti, M., Gatt, A., & Camilleri, K. P. (2018). Where to put the image in an image caption generator. Natural Language Engineering, 24(3), 467-489.
