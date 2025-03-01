# Bone_age_prediction_W_net
we used the hybrid model with unsupervised pretrained model with w-net for segmentation and using transfer leaning to predict the bone age with hand radiographs.the codes is in the notebook .
# idea descriptions
In thhis repository , at first i implemented a w-net on the radiographs of the hand and i trained it as a unsupervised segmentation model. then i saved the first part of the model as a feature extractor for the hand radiographs, after that i added 5 layer of fully connected layers to predict the age and trained it supervised manneer.
bottlenecks of the project:
the important bottle neck is that for such a unsupervised model i need trainig for really high number of epochs and gpu resources.
This is the w-net architecture .
![image](https://github.com/user-attachments/assets/15bd3474-59bb-4d41-835b-d9bf68ddcfb9)
the idea which we used is that we trained an unsupervised model to extract the features and then we connect it to some fully connected layers to predict the bone ages.
here is the training results
![w-net_results](https://github.com/user-attachments/assets/6a47305b-3e9a-4362-ba3c-674c14daa75b)
as you can se in both models , the pre-trained one and the hybrid one the loss function is decreasing during the training. at the bottom you can see some pre-processed results and some EDA on the luminance of the images.
