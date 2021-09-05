# Handwritten-Hindi-Word-Recognizer

There are three steps in recognition which are pre-processing, feature extraction and classification.
We adopt the divide-and conquer policy wherein a major category is divided into sub-categories thus making the classification process simpler. 
Segmentation is the important step. Segmentation also contains three major steps such as line segmentation, word segmentation and character segmentation. If we fail in doing line segmentation then entire segmentation process goes wrong.


We start with loading the image using load_image function then remove major noise and shadows using adaptive thresholding method on the original image using remove_noise_and_preprocess function. For further cleaning the image, we first resize the image to 50% of it’s original size using makesmall function, then we apply simple thresholding methods like Thresh_binary, thresh_OTSU. We then apply morphological operation Opening so that the image looks better using preprocess function. 







