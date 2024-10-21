# multimodal_damage_image_selector
This is a binary image classification model that identifies whether an image depicts damage or non-damage. It uses InceptionV3 as a feature extractor (via transfer learning) and adds custom dense layers to adapt the model to the new task. The model is compiled with the Adam optimizer and binary crossentropy loss to optimize performance.

The accuracy of this model is 85.5%. This correctly classifies most images, but there is room for improvement. Some ways this can be improved is to adjust the learning rate or increasing/decreasing the batch size, or training more dense layers.

This code also randomly selects an image from the test set and uses the trained model to predict its class (either 'damage' or 'non-damage'). It then displays the image with both the actual label and the predicted label for comparison.

