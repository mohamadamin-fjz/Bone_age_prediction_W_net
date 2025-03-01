# Bone_age_prediction_W_net
we used the hybrid model with unsupervised pretrained model with w-net for segmentation and using transfer leaning to predict the bone age with hand radiographs.
# idea descriptions
In thhis repository , at first i implemented a w-net on the radiographs of the hand and i trained it as a unsupervised segmentation model. then i saved the first part of the model as a feature extractor for the hand radiographs, after that i added 5 layer of fully connected layers to predict the age and trained it supervised manneer.
bottlenecks of the project:
the important bottle neck is that for such a unsupervised model i need trainig for really high number of epochs and gpu resources.
The training reults and plots is on the results jpeg file

