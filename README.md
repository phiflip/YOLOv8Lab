# YOLOv8Lab
<img src="https://github.com/phiflip/YOLOv8Lab/blob/main/icons/YOLOv8Lab_final_icon_nobackgorund_highRes.png" width="200" alt="ModVegePy main logo type">
</div>
Welcome to the YOLOv8Lab repository, a dedicated platform for setting up and using YOLOv8 for object detection tasks in educational settings. This repository serves as a hub for individuals interested in configuring and deploying YOLOv8 for custom object detection.

## Installation

This project assumes that Anaconda and Spyder are installed on your Windows system. Follow the steps below to set up your environment.

### Prerequisites

- Anaconda: Download and install Anaconda from the [official website](https://www.anaconda.com/products/individual) ([Installing on Linux](https://docs.anaconda.com/free/anaconda/install/linux/), [Installing on macOS](https://docs.anaconda.com/free/anaconda/install/mac-os/).)
- Python 3.9

### Directory structure

1. **Create the yolov8 project folder**
```bash
C:/
├─ Users
│   ├─ UserName
│   │   ├─ yolov8                  
│   │   │   ├─ labeling/        
│   │   │   ├─ train/
│   │   │   ├─ test/     
│   │   │   └─ valid/
│   │   └─ ...             
│   └─ ...
└──...
```
### Environment Setup (via Anaconda Prompt)

2. **Create a new conda environment (in the windows search bar type "Anaconda Prompt"):**
   ```bash
   conda create --name yolov8 python=3.9 spyder=5
   ```

3. **Activate the environment:**
   ```bash
   conda activate yolov8
   ```

5. **Install Required Packages:**
   ```bash
   pip install ultralytics
   ```

6. **Launch Spyder within the new environment:**
   ```bash
   spyder
   ```
7. **… and check your installation by opening and running the yolov8_test.py in spyder:**
   
   [Download yolov8_test.py](https://github.com/phiflip/YOLOv8Lab/blob/main/scripts/yolov8_test.py)

### Additional Tools

1. **Install labelImg for image annotation using the same activated yolov8 environment:**
   ```bash
   conda install -c conda-forge labelimg
   ```
2. **Start the labeling software:**
   ```bash
   labelImg
   ```

## Usage

In this repository, you will find various CLI snippets that help perform basic tasks such as trainings and predictions on datasets.

## Most important command line interface (CLI) commands
### run an pretrained yolo object detector on your webcam
```bash
yolo predict model=yolov8n.pt source=0 show=True
```
## Test Dataset

A test dataset is included in the `data/test` directory. This can be used to verify the functionality of YOLOv8 in case theres no custom dataset available.
