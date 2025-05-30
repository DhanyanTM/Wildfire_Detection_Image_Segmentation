# Wildfire_Detection_Image_Segmentation
This project explores the application of deep learning-based semantic segmentation to improve wildfire detection accuracy and real-time monitoring.

Overview of Approach:
This project explores the application of deep learningbased semantic segmentation to improve wildfire detection
accuracy and real-time monitoring. We aim to develop a
model that can process aerial and satellite imagery to detect
and delineate fire-affected regions. Our approach involves:

• Data Preprocessing: Annotating wildfire images, applying data augmentation techniques, if necessary.

• Model Selection: Evaluating convolutional neural network (CNN) architecture like U-Net and
transformer-based architectures such as Segformer,
leveraging backbone networks like ResNet and EfficientNet.

• Training and Loss Optimization: Using Dice Loss or
Weighted Binary Cross-Entropy Loss to address class
imbalance between the background pixels and the fire
pixels.

• Evaluation Metrics: Some common metrics for semantic segmentation that we chose to use include IoU,
Precision, Recall, F1 Score, False Positive & False
Negative Rates, Pixel Accuracy, and Inference Speed.

Dataset
• Source: IEEE DataPort FLAME Dataset.
• Size: This dataset consists of 2,003 fire frames with a
resolution of 3480x2160. The size of this repository is
5.3 GB and the format is JPEG. It also includes 2,003
JPEG files of ground truth masks, which was 23.4 MB.

My Inference:
Although SegFormer has strengths in precision and efficient representation learning, UNet proves to be the better
candidate for wildfire detection, primarily due to its superior recall and segmentation completeness. The negligible increase in false positives is an acceptable compromise
given our higher priority to detect all possible fire instances
with minimal latency. UNet is more suited for deployment
in high-risk, real-time wildfire monitoring systems, where
missing even a single instance of fire can have devastating
consequences.
