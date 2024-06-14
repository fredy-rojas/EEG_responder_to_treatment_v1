# Identifying Responders to Spinal Manipulation Therapy Using EEG Patterns and Deep Learning

## ResNetv2 - Feature Map Visualization - Alpha brainwave signal:
![ResNetv2_Feature Map VIZ](_images/FR_ResNetv2_FeatureMap_v1.gif)

Usually, digital images have 3 channels (Red, Green, and Blue), meaning that a pixel within an image will have 3 values. The ResNet architecture increases the number of channels (feature maps) in the images while decreasing the spatial dimensions (height and width of the pixels) to extract relevant patterns that help with the classification task.

Feature map visualization is a way to look inside this architecture to understand what is happening with the input. Since it is not possible for humans to interpret an image with a large number of channels, at each dimension reduction step within the architecture, I create an average of all those channels to produce the visualizations.

The figure shows the EEG epoch topoplots for an individual who has responded positively to SMT (spinal manipulative therapy) and another who has not. As shown on the left-hand side of the image, the topoplots appear almost identical to the naked eye. However, at the last stage of the architecture, it was able to highlight differences, which are then used to feed a fully connected layer for classification.
