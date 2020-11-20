# Android-Age-Classification
Age Classification App using Native Android. The quantized .tflite model was trained and generated using [TensorFlow Lite Model Maker](https://www.tensorflow.org/lite/tutorials/model_maker_image_classification).
Face databases used: [UTKFace](https://susanqq.github.io/UTKFace/) combined with [Appa-Real](http://chalearnlap.cvc.uab.es/dataset/26/description/).

## Model description

Classes used (based on [The 12 Stages of Life](https://www.institute4learning.com/resources/articles/the-12-stages-of-life/) article):
- 04 - 06 years old - *early childhood*
- 07 - 08 years old - *middle childhood*
- 09 - 11 years old - *late childhood*
- 12 - 19 years old - *adolescence*
- 20 - 27 years old - *early adulthood*
- 28 - 35 years old - *middle adulthood*
- 36 - 45 years old - *midlife*
- 46 - 60 years old - *mature adulthood*
- 61 - 75 years old - *late adulthood*

## Setting up the project
- Download and install [Android Studio](https://developer.android.com/studio#downloads)
- Clone this repository

```
git clone https://github.com/radualexandrub/Android-Age-Classification.git
```

- Delete all `.iml` files within the project folder (Search for `.iml` files and delete all of them). [This will solve `Unsupported Modules Detected:` Error](https://stackoverflow.com/questions/28668252/android-studio-error-unsupported-modules-detected-compilation-is-not-supported)
- Open Android Studio and click on `Import Project (Gradle, Eclipse ADT, etc.)` (Do **not** click on `Open an Existing Project`)
- Wait for Gradle to set up all the required packages
- If Error [`Gradle sync failed: Module: 'app' platform 'android-29' not found.`](https://stackoverflow.com/questions/60681045/error-module-app-platform-android-28-not-found-and-design-editor-is-unava) is encountered, go to `File -> Settings -> System Settings -> Android SDK -> Check Android 10.0` and hit `Apply`. After installation, click on `File -> Sync Project with Gradle files` and wait for it's setup.
- Click on `Run 'app' (Shift+F10)`
- If Error [`Unable to delete file`](https://stackoverflow.com/questions/47312169/android-studio-3-0-unable-to-delete-file/47312259) is encountered, just go to the specified directory and delete the file manually. Re-run the project.

## Credits and Resources used:
- [UTKFace Database with age, gender, and ethnicity annotations](https://susanqq.github.io/UTKFace/)
- [APPA-REAL Database that contains 7,591 images with associated real and apparent age labels](http://chalearnlap.cvc.uab.es/dataset/26/description/)
- [TensorFlow Lite Model Maker Library](https://www.tensorflow.org/lite/tutorials/model_maker_image_classification)
- [Pre-made image classification App using Tensorflow Lite](https://blog.notyouraveragedev.in/android/image-classification-in-android-using-tensor-flow/)
