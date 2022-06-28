# firescape

This is a tool that uses a convolutional neural network (YOLOv3) and unsupervised learning in combination with EO satellite images and land use data to identify wildfire hazards in suburban environments.

See https://docs.google.com/presentation/d/1VQKiAySuzwstStzqIDLWofr1tUOQBVP0PZXtW9bN4Yg/edit?usp=sharing for details.

The front end is built in streamlit.

Users enter an address. A fuzzy match finds the location of interest and sources land use data and a satellite image. A pretrained detection model (YOLOv3) is used in tandem with k-means clustering to semantically label trees and identify potential fire hazards.

Why didn't I just use a semantic segmentation model? I didn't have labels and I only had two weeks! The clustering works well. 
