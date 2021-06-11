# Challenge 3: Facial Expression Classification

Deadline: 11.06. 18:00 

Handed in: 

## Solution

### serious solution

Our solution can be found in [Challenge-3-Notebook.ipynb](Challenge-3-Notebook.ipynb) and the predictions can be found in [ToTheMooners_prediction.csv.](ToTheMooners_prediction.csv)

In the jupyter notebook we documented our process, where we did a ususal train-test-split and trained an image regressor with the automatic implementation of keras (called autokeras). This automatic implementation trained for several days to find the best hyperparameters in 100 tries with 1000 epochs for each try.
After training for roughly 3 days, we evaluated on the test set and obtained an accuracy of 100%.

Feedback is highly appreciated!


### fun solution

After obtaining an 100% accuracy we wanted to have some fun and tried another approach. The idea was the following:


1. Extract faces of Prof. Petersen from the frames of the recordings of lectures with the FaceNet 
   network (https://github.com/timesler/facenet-pytorch).
2. Convert the numpy array into a format we can train our CycleGAN in the next step which are 
   jpg images in RGB.
3. Train a petersen2smiley CycleGAN (https://github.com/LynnHo/CycleGAN-Tensorflow-2) between Prof. Petersen 
   and the Facial Expressions.
4. After doing the inference we still have the annotated data - now having a face of Prof. Petersen 
   corresponding to a facial expression. 
5. We would now use the Autokeras (https://autokeras.com/) library to train the classifier in the usual way.

Problems that arose with this type of generative adversarial network is the very long training time to even get reasonable results (we trained on one middle class GPU).
We sadly were not able to fully execute our plan, so we just present some of the more interesting results of the CycleGan.

The extraction of the faces can be found in [face_extraction.ipynb](face_extraction.ipynb). The process --- insert rest ---.
In [petersen2smiley.ipynb](petersen2smiley.ipynb) some examples of the Cyclegan process can be found.



