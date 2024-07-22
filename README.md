# Identifying Responders to Spinal Manipulation Therapy Using EEG Patterns and Deep Learning

## ResNetv2 - Feature Map Visualization - Alpha brainwave signal:
![ResNetv2_Feature Map VIZ](_images/FR_ResNetv2_FeatureMap_v1.gif)

### Objective:
- To determine if ResNet can be used as a prognostic tool for identifying individuals who are likely to respond positively (reduce pain levels) to care.
  - Providing this type of information beforehand to practitioners can help them in the decision-making process to design care plans for patients, improve patient outcomes, and reduce healthcare costs.

### Figure Description:
- The image shows a trained ResNet architecture processing EEG topoplots of two patients, sID_23 and sID_17. On the left, you can see the EEG topoplots (each topoplot represents 2 seconds of EEG recording), and on the right, the probability score output. A probability score above 0.5 indicates that the subject is likely to respond positively to the care plan.
- The EEG topoplot images from left to right (feature maps average) provide insight into how the trained ResNet transforms topoplots to provide a probability score outcome. Notably, to the naked eye, the EEG topoplots for sID_23 and sID_17 look alike. However, in the last stage of the feature maps, the architecture highlights different patterns that are used in a dense layer to create the probability score.
