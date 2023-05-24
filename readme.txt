1. put all the .ipynb , .csv and folder in the same path. Then, run below code one by one.

2. "preprocess.ipynb" : modify the input,output and label .csv path.
                       This code is to combine , crop , normalize and resize the image.

3. "augmentation_test.ipynb" : modify the input,output path
                               This code is to generate augmentation image and save it.

4. put your dataset in below folder structure, suggest split 80% for training and 20% for val randomly.

  3D-CNNs-PE----train----nr
              |        |
              |         --pe
              |
              |--val-----nr
              |       |    
              |        --pe
              |
              |--test-----nr
                      |    
                       --pe 
 
5.  "CT_224_160_48.ipynb" : modify the train ,val path and the model name.
                            This code is to train the 3D CNNs model. 
                            The default patience is 15, it can be adjusted in this case.
                            You can also manually stop , adjust the learning rate and resume the training.


6.  "acc_1_1.ipynb" : modify the val path and the model name.
                      This code provide all the metrics for evalution.

7.  "metrix.ipynb" : This code is for cross validation ,input all the metric from different fold.

8.  Result folder shows my best cross validation result for all fold.
