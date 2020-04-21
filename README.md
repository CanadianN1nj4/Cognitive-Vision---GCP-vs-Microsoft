# Cognitive-Vision---GCP-vs-Microsoft

GCP AutoML Vision Tutorial

This tutorial follows a tutorial done by google but all done using the UI https://cloud.google.com/vision/automl/docs/edge-quickstart.
The rest of the steps are written below. This is a tutorial for the AutoML vision
1.	Go to the google cloud console and create a new project
a.	Make sure billing is enabled on the project when you create it
b.	Enable the AutoML and Cloud Storage APIs
2.	Create a service account
3.	Create a IAM policy for your project where the member is the new service account and the role is automl.editor
4.	Create a cloud storage bucket
a.	Make sure to select the location type as Region and choose us-central1, standard storage and fine-grained access.
5.	Copy any images that you have and want to test into your storage bucket if you have a csv
a.	If you don’t have a CSV for the images, separate the images into folders and zip them with the name of the label, don’t upload
6.	Go to the AutoML Vision UI
a.	Create a new dataset
b.	Import the CSV if you have one
i.	If you don’t, import the project zip files one by one off of your local computer
c.	Wait for the images to load
d.	If you have any unlabeled images left, label them
7.	Train your model
a.	Choose the type of model you want, if you’re going for cloud, choose cloud-hosted, if you’re going for anything else, choose edge
b.	Choose the model that you want based off of the different trade-offs
c.	Set the amount of hours to train your model
d.	Press Train!
8.	Tada, done!


A link to a video of my tutorial: 
https://youtu.be/_sGJ9lc2o04
