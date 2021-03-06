#  <img src="/icons/augmented-reality.png" width="60" vertical-align="bottom"> Patient movement detection prototype
> This project has been developped as part of the Medical augmented reality (IN2293) class at TUM (Technische Universität München). The project consists of a patient movement detector prototype. Given a set of images, the goal was to detect any movement of the object of interest, in that case the patient's arm. The UI had to inform the surgeon that the patient's arm had moved and the degree and localisation of that said movement. To do that, a segmentation using HSV skin's color range had been done, following by some morphological operations. The resulting mask was used as input for the optical flow algorithm. That algorithm gives the movement vectors and magnitudes that were colored and added to the original images.

### Patient movement density
> The goal of the detector was to automatically detect patient's movement during a fake arm surgery. To do so, images of the patient were analyse using [OpenCV](https://opencv.org/). First, a binary mask of the patient's arm was created. Then, the mask was applied to the image and the movement density was estimated.
> <p align="center"><img src="/images/movement_density.PNG" width="600" vertical-align="bottom"><p>
  
### Movement detection from patient's image
> The movement amplitude and angle is applied to the original image in order to intuitively visualize the movement of the patient. The computation of the movement is done using [OpenCV Dense Optical Flow Algorithm](https://docs.opencv.org/3.4/d7/d8b/tutorial_py_lucas_kanade.html)
> <p align="center"><img src="/images/movement_detection.PNG" width="600" vertical-align="bottom"><p>
  

#### How to contribute ?
- [X] Create a branch by feature and/or bug fix
- [X] Get the code
- [X] Commit and push
- [X] Create a pull request

#### Branch naming

##### Feature branch
> feature/ [Short feature description] [Issue number]

##### Bug branch
> fix/ [Short fix description] [Issue number]

#### Commits syntax:

##### Adding code:
> \+ Added [Short Description] [Issue Number]

##### Deleting code:
> \- Deleted [Short Description] [Issue Number]

##### Modifying code:
> \* Changed [Short Description] [Issue Number]


Icons made by <a href="http://www.flaticon.com/authors/freepik" title="Freepik">Freepik</a> from <a href="http://www.flaticon.com" title="Flaticon">www.flaticon.com</a> is licensed by <a href="http://creativecommons.org/licenses/by/3.0/" title="Creative Commons BY 3.0" target="_blank">CC 3.0 BY</a>
