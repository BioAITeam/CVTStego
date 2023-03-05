# CVTStego-Net: a convolutional vision transformer architecture for spatial image steganalysis


In recent years, the leading research in the field of image steganalysis has focused on
convolutional neural network (CNN) architectures, which obtain good results in classifying stego and
cover images. Existing CNNs are increasingly robust and stable; stacked convolutional layers increase
the local receptive field of steganographic noise without taking into account global steganographic noise.
Visual transformers focus attention on processing long-range global dependencies. Visual transformers
require a larger dataset than usual, and this is because, unlike CNNs, it does not have inductive biases
(such as convolutions for processing images). This research presents a convolutional visual transformer
for steganalysis that combines the advantages of convolutions and the benefits of attention mechanisms,
capturing both local and global dependencies. The proposed network is validated on two public image
datasets (BOSSbase 1.01 and BOSSbase+Bows2). Experimental results demonstrate that convolutional
vision transformers can classify steganographic images. This work improves classification accuracies on
all algorithms and bits per pixel (bpp), reaching 86.58% on WOW with 0.2 bpp and 93.80% on WOW
with 0.4 bpp, 80.70% and 90.45% on S-UNIWARD (0.2 and 0.4 bpp respectively), 74.70% and 81.48% on
MiPOD (0.2 and 0.4 bpp), 76.70% and 85.80% on HILL (0.2 and 0.4 bpp), 78.20% and 86.98% on HUGO
(0.2 and 0.4 bpp), using BOSSbase 1.01 test data


## Folders
- **training with TL** this folder contains the codes required to perform the training with transfer learning and multispectral images (15 channels), which contains the python file (code_15channels_with_weights.py) in which the experiments will be run and the file (models_classification2.py) that will contain the models, to be called by the main code.

- **training without TL** this folder contains the codes required to perform the training without transfer learning with multispectral images (15 channels), which contains the python file (code_15channels_without_weights.py ) in which the experiments will be run and the file (models_classification5.py) that will contain the models, to be called by the main code.


## Requirements
This repository requires the following libraries and frameworks:

- TensorFlow 2.10.0
- scikit-learn
- numPy 
- OpenCV 
- Matplotlib
- Time
- os
- scikit-image
- glob


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