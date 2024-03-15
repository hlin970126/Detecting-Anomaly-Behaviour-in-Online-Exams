# Detecting-Anomaly-Behaviour-in-Online-Exams

# What is this project about?
This project tries to detect anomaly behaviours (i.e., potential cheating behaviours) in the environment of online exams

# What does it do?
It currently reads from 10 second video clips (supports mp4 format) and detects whether there exists certain frames that the candidate in the video is involved in cheating.

# How does it work?
We apply the combination of convolutional neural network together with LSTM to extract features of potential anomaly behaviours.

# How does it perform?
70% average accuracy for our collected dataset, 8 to 9 seconds prediction for each 10-second video frame

# What does each file do?
The data_to_tensors file reads from google drive and unpacks videoes into data tensors.
The behviour_detect file trains on the dataset and makes a model for prediction

# How can it work with different datasets?
You can either re-train the model by using own data, or use the existing model from https://drive.google.com/drive/folders/1st8YnN30R6NN2pOdk4kpKY9SRuqFF7HN?usp=drive_link, run the model converging method in behaviour_detect, and use the combined model for own testing
