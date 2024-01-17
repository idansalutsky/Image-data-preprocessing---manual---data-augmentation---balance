# Preprocessing_image_data-manual-data-augmentation-balance

The purpose of this task is, given a fixed ML model of image labeling, to do preprocessing to the image data to improve the model's results.
The images are part of the data of MNIST (database of handwritten digits).
First, we manually went through the images and filtered out from the various digits images that were not digits at all, i.e. drawing or gibberish, and labeled digits that were clearly mislabeled.

In addition, after the manual transition, we performed various augmentations to the data in order for the model to learn it in different situations such as rotation every 90 degrees, blurring cutting and combinations thereof.

Finally, in order for the model not to be biased due to the data itself, we balanced the number of images in each digit and sampled from each folder of each digit the number of examples as the number of examples in the digit that had the minimum number of images.

The results did improve the model both in accuracy and in the F1 index.
