# CVTStego-Net: a convolutional vision transformer architecture for spatial image steganalysis


The principal investigations in image steganalysis in the spatial domain have concentrated on convolutionalneural network (CNN) designs. However, existing CNNs increase the local receptive field of steganographicnoise without considering global steganographic noise. This study introduces CVTStego-Net, a convolutionalvision transformer for spatial domain image steganalysis that merges the strengths of convolutions andthe advantages of attention mechanisms to capture both local and global dependencies. CVTStego-Net iscomposed of three stages: preprocessing stage, noise extraction, and analysis stage, and classification stage. Thepreprocessing stage involves a bifurcation with trainable and untrainable 30 SRM (Spatial Rich Models) filtersto enhance steganographic noise. The noise extraction and analysis stage combines the SE-Block (Squeeze-and-Excitation) with residual operations to increase the sensitivity to steganographic noise and suppressingthe influence of redundant information, and the classification stage combines SE-Block with a convolutionalvision transformer to connect the local and global spatial relationships of the steganographic noise. This workenhanced the classification accuracies for steganographic algorithms compared to YEDROUDJ-Net, SR-Net,ZHU-Net, GBRAS-Net, and SNMC-Net. Specifically, the accuracy of CVTStego-Net for WOW at 0.2 bpp was 86.58%, and 0.4 bpp was 93.80%. Moreover, for S-UNIWARD at 0.2 and 0.4 bpp, the accuracies were 80.70%and 90.45%, respectively. For MiPOD at 0.2 and 0.4 bpp, the accuracies were 74.70% and 81.48%, respectively.For HILL at 0.2 and 0.4 bpp, the accuracies were 76.70% and 85.80%, respectively, and for HUGO at 0.2 and0.4 bpp, the accuracies were 78.20% and 86.98%, respectively, using test data from the BOSSbase 1.01. Theresults demonstrate that convolutional vision transformers can classify steganographic images in the spatialdomain.


## Folders
- **transformer_1.py** This file contains the model used in the various training experiments carried out for the research. To use it, the database must be varied and the hyperparameters adjusted to obtain the desired results, while keeping the same code.

- **SRM_Kernels1.npy** This file contains the weights of the 30 SRM high-pass filters used for model training.

## Requirements
This repository requires the following libraries and frameworks:

- TensorFlow 2.10.0
- scikit-learn
- numPy 
- OpenCV 
- Matplotlib
- os
- scikit-image



This repository was developed in the Python3 (3.9.12) programming language.


## Authors
Universidad Autonoma de Manizales (https://www.autonoma.edu.co/)

- Mario Alejandro Bravo-Ortiz 
- Esteban Mercado-Ruiz 
- Juan Pablo Villa-Pulgarin 
- Harold Brayan Arteaga-Arteaga
- Reinel Tabares-Soto 



## References

[1] 
