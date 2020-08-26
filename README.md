# 3D Barin tumor segmentation tensorflow Keras

## Background




### Training
1. Download dataset [BRATS 2018 competition page](https://www.med.upenn.edu/sbia/brats2018/registration.html).
unzip and place in your computer add the path of the folder in new_train.py folder

2. Install Python 3 and dependencies: 
```
nibabel,
keras,
pytables,
nilearn,
SimpleITK,
nipype
```
(nipype is required for preprocessing only) 

3. preprocess.py give the path of your data-set folder to preprocess the image
6. Run the training:

To Start training the model:
```
$ python New_train.py
```
you can also download pretrained model from
[Here](https://drive.google.com/file/d/1ylYeJ4fxDbSpLrVQB3hLkg6i9_HsZAnv/view?usp=sharing)



### Write prediction images from the validation data

```
$ python new_model_prediction.py
```
The predictions of our pretrained model is in the ```prtV``` folder along with the input data and ground truth labels for 
comparison.
I have also uploded the pretrained model prediction outputs and each dice score in the pretv folder.
you can download all outputs from 
[Here](https://drive.google.com/file/d/11iQMOGd3moDCxTwtrYIButIVvgeO36Z0/view?usp=sharing)





For Evaluation Run evaluate.py




## Citations
GBM Data Citation:
 * Spyridon Bakas, Hamed Akbari, Aristeidis Sotiras, Michel Bilello, Martin Rozycki, Justin Kirby, John Freymann, Keyvan Farahani, and Christos Davatzikos. (2017) Segmentation Labels and Radiomic Features for the Pre-operative Scans of the TCGA-GBM collection. The Cancer Imaging Archive. https://doi.org/10.7937/K9/TCIA.2017.KLXWJJ1Q

LGG Data Citation:
 * Spyridon Bakas, Hamed Akbari, Aristeidis Sotiras, Michel Bilello, Martin Rozycki, Justin Kirby, John Freymann, Keyvan Farahani, and Christos Davatzikos. (2017) Segmentation Labels and Radiomic Features for the Pre-operative Scans of the TCGA-LGG collection. The Cancer Imaging Archive. https://doi.org/10.7937/K9/TCIA.2017.GJQ7R0EF
