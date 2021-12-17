# UAPET - Underwater Animal Pose Estimation and Tracking

UAPET is ___. It supports object detection, pose estimation, and interaction classification models, and is trained on sycronous camera video data from underwater cameras at the Brookfield zoo in Chicago, Illinois.

## Features:

* Machine-learning supported labeling tool GUI for rapidly labeling large datasets for object detection, pose estimation, and interaction classification models.
* Object detection models trained using prebuilt and custom workflows.
* Pose estimation models trained using [SLEAP](https://sleap.ai/) and [DeepLabCut](https://github.com/DeepLabCut/DeepLabCut), using both top-down and bottom-up approaches.
* Interaction classification models labeled using UAPET tool, with support for several increasing levels of complexity and assumption.

## File structure:
The 'old' folder contains the original UAPET code, which is no longer maintained and is included for reference only.

```bash
├── old
|   ├── [...]
├── TensorFlow
|   ├── addons
|   |   ├── tensorflow_addons
|   ├── models
|   |   ├── object_detection
|   ├── workspace
|   |   ├── annotations
|   |   ├── exported-models
|   |   ├── images
|   |   |  ├── train
|   |   |  ├── test
|   |   ├── models
|   |   ├── pre-trained-models
|   |   ├── videos
├── README.md
├── requirements.txt
└── bibliography.bib
```

## Getting Started:
<!-- 
To view the tool locally in a browser, click [HERE].  -->

Running the tool locally requires the following installations:

1. [Python 3.8](https://www.python.org/downloads/)
2. [Anaconda](https://www.anaconda.com/)

To access the code repository or run the tool locally, complete the following steps:

1. Clone this repository (either from command line or from [GitHub](https://github.com/Bailey-Man/UAPET)
2. Navigate to the cloned repository using command line
3. Create an Anaconda environment to contain the workspace using the following commands:
```bash
    conda create -n uapet_env python=3.9
    conda activate uapet_env  
```
4. Use pip to install all required package dependencies: 
```bash
    pip install -r requirements.txt
```
5. The all-purpose labeling tool notebook is available [HERE](LabelTool.ipynb), the notebook evaluating Object Detection is available [HERE](ObjectDetection.ipynb), the notebook evaluating pose estimation is available [HERE](PoseEstimation.ipynb), and the notebook evaluating interaction classification is available [HERE](InteractionClassification.ipynb).
6. Further instructions are contained within each respective jupyter notebook


## Contributions:
Code was originally developed by [Bailey Man](https://www.linkedin.com/in/bailey-man/), as part of the [HDSI Undergraduate Scholarship project](https://datascience.ucsd.edu/congratulations-2021-hdsi-scholarship-recipients/).The program (and as an extension this project) are funded by the [Halıcıoğlu Data Science Institute](https://datascience.ucsd.edu/) The project began development in January 2021 and was submitted in December 2021, with future work contingent on available time and funding in the coming year. 

The project was developed in conjunction with the help of several mentors: 
* [Zhen Zhai](https://www.linkedin.com/in/zhenzhai/)
* [Dr. Ilya Zaslavsky](https://www.linkedin.com/in/ilya-zaslavsky-7997ab7/)

UAPET is open-source project and tool, and has benefited from suggestions and contributions from the community. In particular, the following people have provided invaluable feedback and support:
* [Dr. Christine Johnson](http://hci.ucsd.edu/people/johnson/)
* [Eric Leonardis](https://www.linkedin.com/in/eric-leonardis-a6225042/)
* [Jeremy Karnowski](https://www.linkedin.com/in/jeremykarnowski/)


## References

Below is a brief list of links to publications that are used or were referenced in the creation of UAPET.

* [SLEAP](https://sleap.ai/)
* [DeepLabCut](https://github.com/DeepLabCut/DeepLabCut)
* [Quantifying Behavior](https://www.nature.com/articles/s41593-020-00734-z.epdf?sharing_token=cqf_3nZnHvh46f_kpkBSyNRgN0jAjWel9jnR3ZoTv0OPIwFGiZW1SPpUQnvK5VQTg9HkeG-0CxD-HJhNZskWIzJOprb8q6n4gbkYKV_DT1RSQTvXXn92QzdKZyo29n9OXnS2dec3oqoKMThPE4OYvovg8dAE4rr0sfFvMeHGj2k%3D)
* [TensorFlow](https://github.com/tensorflow)
* [CNN Dolphin Images](https://link.springer.com/chapter/10.1007/978-3-030-01171-0_22)
* [CNN Risso's Dolphins](https://www.researchgate.net/publication/340967995_Convolutional_Neural_Networks_for_Risso's_Dolphins_Identification)
* [InceptionV3](https://keras.io/api/applications/inceptionv3/)
* [InceptionResNetV2](https://keras.io/api/applications/inceptionresnetv2/)

A full list of resources can be found in BibTeX format in the [Bibliography](bibliography.bib) file.

## License: 

This software is produced under the MIT License.

Copyright (c) 2021 Bailey Man

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
