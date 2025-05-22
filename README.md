For this project to run we need python 3.10
Install the modules from requirements.txt
./runs contains all graphs of training/validating. Run via commann "tensorboard --logdir runs" to see graphs.
./Results contains notebook files from different runnings. To identify the graph for this particular run, look at printed timestamp inside the notebooks.
Use Make_dataset_with_mtcnn.ipynb to create dataset with cropped faces using MTCNN.
Use Embedding-view.ipynb to see embeddings in 2-dimesnional space with VOXEL51 fiftyone module. Note that it usess .pt file to upload models weights, so please, first try to train a model.
For training run ResNet18-CASIA-train.ipynb
