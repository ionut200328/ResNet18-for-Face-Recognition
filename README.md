# ResNet18-for-Face-Recognition

To download CASIA-WebFace or other face recognition datasets follow https://github.com/deepinsight/insightface/tree/master/recognition/_datasets_#casia-webface-10k-ids05m-images-1

After downloding the dataset, use a detection model (MTCNN in our case) to create a new dataset of same structure, but with croppped faces.

For training use ResNet18-CASIA-train.ipynb. Note that you can manually adjust the parameters by updating the seconds cell constants. You need to modify the paths in the functions to use your dataset.

For testing use ResNet18-LFW-testing.ipynb. You need to also use a detection model to crop the faces and create a new dataset with them. Also, paths may need adjustment.

With Embedding-view.inpnb you can see the embeddings (in reduced dimensionality) using the FiftyOne framework. It supports uploading standard LFW dataset via FiftyOne. The faces are then cropped usin MTCNN and further passed to the model. 
