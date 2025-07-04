# TESRGAN
This project focuses on restoring and enhancing the quality of degraded historical images using Generative Adversarial Networks (GANs). By leveraging the capabilities of deep learning, particularly a custom hybrid model named TESRGAN (Transformer-Enhanced Super-Resolution GAN), the approach combines GAN architecture with transformer components to generate high-resolution reconstructions. The model is trained on a diverse dataset of old and damaged images to learn semantic details and visual patterns. The outcome is significantly improved image clarity, preserved structural integrity, and realistic restoration, offering a valuable tool for digital archiving, cultural preservation, and historical research.
## Dataset 
For training, COCO dataset (voxel51/coco-2017 available on  http://cocodataset.org/#home) is used, pair of low-resolution (LR) and high-resolution (HR) images is utilized. 
The HR images are downsampled using bicubic interpolation by a factor of 4 to create the corresponding LR inputs.  
The dataset is divided into  Train2017: This subset contains 118K images for training object detection, segmentation, and captioning models, and 
Val2017: This subset has 5K images used for validation purposes during model training.

To evaluate TESRGAN’s effectiveness in its target application, a custom dataset is created comprising of 200 historical images used for testing are available individually on https://kamat.com//kalranga/itihas/history.htm. This dataset consists of digitally scanned photographs, manuscripts, and archival images with varied degrees of degradation such as noise, blurring and low contrast. 
