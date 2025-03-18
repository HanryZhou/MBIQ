# MBIQ Dataset

The **MBIQ (Motion Blur Image Quality)** dataset is a motion blur image quality database designed to address the lack of existing databases that focus on motion blur in image quality assessment. This dataset contains high-quality images captured under controlled motion blur conditions with quantitative ground truth labels.



##  Dataset Overview

- **Name**: MBIQ (Motion Blur Image Quality Database)
- **Number of Images**: 50 images
- **Number of Scenes**: 10 distinct scenes, with 5 images per scene
- **Scenarios**: Indoor and outdoor scenes under various lighting conditions

​	The database was generated using a systematic process to ensure reproducibility and consistency. The blur level is quantified based on the turntable rotation speed, offering a precise and objective measurement of motion blur intensity.



## Generation Process

![generation of MBIQ and examples](assets\generation of MBIQ and examples.png)

1. A **mobile phone camera** with its OIS (Optical Image Stabilization) module turned off is placed vertically on a **rotating platform**.
2. The **rotation axis** of the platform is aligned with the optical center of the camera.
3. The camera’s exposure time, sensitivity, and other settings are kept constant.
4. The platform rotates at different speeds to simulate varying degrees of motion blur.
5. Images are captured sequentially as the rotation speed increased.

**Theory**: There is an approximate linear positive correlation between the blur intensity in the images and the turntable rotation speed, derived from the imaging geometry.



## Dataset Structure

The MBIQ dataset contains the following files:

### Main Files:

- **Images/**: A folder containing all 50 images in high resolution, organized by scene.

- **MBIQ.csv**: A CSV file that provides metadata about the dataset:
  - `name`: Name of the image file.

  - `rotation_period`: The period of the turntable's rotation (in seconds).
  - `rotation_speed`: The speed of the turntable (in degrees/second).

### CSV File Example:

|  name   | rotation_period/s | rotation_speed/(rad/s) |
| :-----: | :---------------: | :--------------------: |
| 1-1.jpg |         0         |           0            |
| 1-2.jpg |       6.57        |         0.956          |



## How to Download

The dataset is available on [Google drive](https://drive.google.com/file/d/1VN705SxvaZPMXVJDI0VXGgFZ4ffl2UKO/view?usp=sharing).



## Citation

Coming soon...

