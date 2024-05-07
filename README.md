# Deploying a Deep Learning model

![image](https://github.com/AbhayPancholi/Object_Detection/assets/114471400/f6799093-88ee-45b9-83f6-07357b46a6ca)

 
## Introduction
Welcome to the Object Detection with YOLOv3 and FastAPI repository!

This project aims to simplify object detection tasks using the powerful YOLOv3 model. Leveraging a pre-trained model, we've developed a straightforward solution for detecting objects in images. The integration of FastAPI streamlines the deployment process, allowing seamless serving of the model.

In this repository, you'll find two essential components: **client.ipynb** and **server.ipynb**. The **server.ipynb** file contains the code to initiate the server locally, enabling easy access to the detection model. Meanwhile, **client.ipynb** basic code to interact with the server, allowing users to submit images and receive annotated outputs swiftly.

Whether you're a beginner exploring the realm of object detection or a seasoned developer seeking a rapid-deployment solution, this repository offers a valuable resource to enhance your projects. Dive in, explore the code, and empower your applications with efficient object detection capabilities.

# How to install and run the project
 
As a general note, the commands are meant to be run within a terminal. To begin you need to **clone this repo in your local filesystem and `cd` to the Object_Detection directory**.

To clone the repo use this command:
```bash
git clone https://github.com/AbhayPancholi/Object_Detection.git
```

or for cloning via SSH use:
```bash
git clone git@github.com:AbhayPancholi/Object_Detection.git
```

If you are unsure which method to use for cloning, use the first one.

The `cd` command allows you to change directories. Assuming you are in the directory where you issued the cloning command, type the following on your terminal.
```bash
cd Object_Detection
```
This will bring you to the `Object_Detection` directory. The `ls` command allows you to list the files and directories.
Type `ls` and let's take a quick look at the content inside `Object_Detection` directory:
 
```
.
└── Object_Detection (this directory)
    ├── images (includes some images from ImageNet)
    ├── server.ipynb (Part 1 of the project)
    ├── client.ipynb (Part 2 of the project)
    └── requirements.txt (python dependencies)
```
 
 
## Python Virtual Environment with Conda
 
### Prerequisites: Have [conda](https://docs.conda.io/en/latest/) installed on your local machine.
 
Use Conda as an environment management system so that all the dependencies you need for this project are stored in an isolated environment.
 
Conda includes a lot of libraries so if you are only installing for this project, we suggest using [miniconda](https://docs.conda.io/en/latest/miniconda.html), which is a minimal version of conda.
 
### 1. Creating a virtual Environment
 
Now we assume that you either successfully installed conda or that it was previously available in your system. The first step is  creating a new developing environment. Let's set a new environment with python 3.8 with this command:
 
```bash
conda create --name object-detection python=3.8
```
 
After successfully creating the environment, you need to activate it by issuing this command:
 
```bash
conda activate object-detection
```
 
At this point, you will do all your libraries installation and work in this environment. So, whenever working on this project, check the object-detection environment is active.

 
### 2. Installing dependencies using PIP 
 
Before proceeding, double-check that you are currently on the `Object_Detection` directory, which includes the `requirements.txt` file. This file lists all the required dependencies and their respective versions. 

Now use the following command to install the required dependencies:
 
```bash
pip install -r requirements.txt
```
 
This command can take a while to run depending on the speed of your internet connection. Once this step is completed you should be ready to spin up jupyter lab and begin working on the project.
 
### 3. Launching Jupyter Lab
 
Jupyter lab was installed during the previous step so you can launch it with this command:
```bash
jupyter lab
```
After execution, you will see some information printed on the terminal. Usually, you will need to authenticate to use Jupyter Lab. For this, copy the token that appears on your terminal, head over to [http://localhost:8888/lab](http://localhost:8888/lab) and paste it there. Your terminal's output should look very similar to the next image, in which the token has been highlighted for reference:


![Token in terminal](./assets/token.png)


### 4. Running the notebook
 
Within Jupyter lab you should be in the same directory where you used the `jupyter lab` command.
 
Look for the `server.ipynb` file and open it to begin the ungraded lab.

To stop jupyter lab once you are done with the lab just press `Ctrl + C` twice.
 
### And... that's it! Have fun deploying a Deep Learning model! :)

 
# 
#
# Acknowledgments:

This project is part of the "Machine Learning Engineering for Production (MLOps)" course offered by deeplearning.ai on Coursera. Special thanks to the instructors and team at deeplearning.ai for their comprehensive curriculum and guidance throughout the course.
