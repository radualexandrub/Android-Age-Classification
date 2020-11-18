# Android-Age-Classification
Age Classification App using Native Android. The quantized .tflite model was trained and generated using [TensorFlow Lite Model Maker](https://www.tensorflow.org/lite/tutorials/model_maker_image_classification).
Face databases used: [UTKFace](https://susanqq.github.io/UTKFace/) combined with [Appa-Real](http://chalearnlap.cvc.uab.es/dataset/26/description/).

## Model description

Classes used (based on the article: [The 12 Stages of Life](https://www.institute4learning.com/resources/articles/the-12-stages-of-life/)):
- 04 - 06 years old - *early childhood*
- 07 - 08 years old - *middle childhood*
- 09 - 11 years old - *late childhood*
- 12 - 19 years old - *adolescence*
- 20 - 27 years old - *early adulthood*
- 28 - 35 years old - *middle adulthood*
- 36 - 45 years old - *midlife*
- 46 - 60 years old - *mature adulthood*
- 61 - 75 years old - *late adulthood*

## Credits and Resources used:
- [UTKFace Database with age, gender, and ethnicity annotations](https://susanqq.github.io/UTKFace/)
- [APPA-REAL Database that contains 7,591 images with associated real and apparent age labels](http://chalearnlap.cvc.uab.es/dataset/26/description/)
- [TensorFlow Lite Model Maker Library](https://www.tensorflow.org/lite/tutorials/model_maker_image_classification)
- [Pre-made image classification App using Tensorflow Lite](https://blog.notyouraveragedev.in/android/image-classification-in-android-using-tensor-flow/)
