This repository has been created to support my MSc project “Automated Assessment of Wheat Crop Health Using RGB Imagery" at the University of Bristol.
The project explores whether convolutional neural networks (CNNs), trained only on RGB images, can classify wheat leaves into Healthy, Septoria, and Stripe Rust, and also predict a continuous health score from 1–10.

How this repository is organised?
The repository is designed to follow the same structure as the experiments described in my thesis.

Data:
The dataset is included here in a folder called data/. Another folder called unseen data/ contains unseen data which was tested on the model.  

Notebooks:
These are the main scripts of the project in the main branch, written as Jupyter notebooks so you can see the code, outputs, and explanations together.
There is another branch named Trails where I've notebooks that i used to buildup on my final main branch. 

1. Performance_Comparision.ipynb – Trains three ResNet models (ResNet18, ResNet34, ResNet50) and compares them.
2. Regressor.ipynb – Uses ResNet50 as a regressor to predict continuous health scores between 1 and 10. Grad-CAM heatmaps to show where the model is looking when making predictions.
3. Exploratory_cross_crop.ipynb – An exploratory test of the wheat-trained model on potato leaves (Healthy, Early Blight, Late Blight) to check generalisation.


How to use this repository?
To get started, you’ll need Python installed. It’s easiest to create a virtual environment so that all packages are contained.

1. Clone this repository to your computer.
2. Open the notebooks in order, starting with labelled_training.ipynb. Each notebook builds on the previous one.
3. The models and results can then be reproduced step by step.

Relation to my MSc Thesis: 
This code was written to generate the experiments, figures, and results that are discussed in my MSc dissertation.

1. The thesis text explains the methods and findings in detail.
2. The notebooks here provide the actual implementation.
3. The dataset is openly available on Kaggle and linked above.
4. Together, they make the project fully reproducible.

This repository is intended as a companion to my dissertation. If you are reading this as an examiner or researcher, please start by browsing the notebooks in order, and cross-reference them with the chapters in the thesis. Each notebook corresponds to a stage of the methodology and results sections.