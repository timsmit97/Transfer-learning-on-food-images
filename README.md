# Transfer-learning-on-food-images
Group project for the master course 'Applied machine learning'. Classification of unstructured data while using applications of transfer learning.









Practical info:
First, we generated different datasets ("bags of images") using "Create_Bags_Of_Images.ipynb".
We then generated random parameters using "Random_Parameter_Generator.ipynb". 
On each bag of images, we trained an InceptionV3 model with these randomly generated parameters. 
Training the models is done using the existing code (via TensorFlow) "retrain.py". 
Retrain.py can be activated using the command line. An example of such a commandline statement is:

Python C:\Users\......\retrain.py 
--image_dir= C:\Users\......\train_set 
--train_batch_size=<integer>
--how_many_training_steps=<integer>
--learning_rate=<float>

After training a model the labels are predicted using "Predict_Labels.ipynb".
Finally, the predictions of the models are combined/stacked using "Stack_Predictions.ipynb". 



In the first weeks of the project we trained models using the "Multiple_Models.ipynb" code. 
However, the results were not accuractely enough. Therefore, we did not use this code at the end.
