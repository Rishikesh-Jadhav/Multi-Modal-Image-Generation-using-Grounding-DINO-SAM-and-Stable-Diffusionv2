# Grounding-DINO-Segment-Anything-Model-and-Stable-Diffusion

<img src="dino_sam_sdiff.png" alt="Results" width="50%">

## Overview
This project focuses on combining Grounding DINO for zero-shot object detection with Meta AI's Segment Anything Model (SAM) for semantic segmentation and finally Stable Diffusion for inpainting the input image . The gaol of the project wast to integrate these techniques and deploy the model on Hugging Face with a Gradio interface for users to detect, segment regions and inpaint them in images. 
NOTE: This application works best for image swith the resolution of 512x512 for images with a higher reolution the inapinting quality drops substantially.

## Key Features

- **Simulation Environment:** Utilized the AirSim simulator for autonomous vehicle control simulation.
  
- **Data Collection:** Gathered sensor data from the simulator, including front-facing camera images and state variables like steering, throttle, speed, and brake.

- **Neural Network Training:** Implemented a multi-layered neural network architecture suitable for control tasks, providing a jittery-free output.

- **Evaluation Metrics:** Assessed model performance using Mean Squared Error (MSE) and qualitative indicators for real-world scenarios.

## Methodology

The project employs a systematic approach to augment conventional PID and MPC controllers with adaptive multi-layered neural networks. The neural network architecture combines convolutional layers for image analysis with additional numerical data, resulting in improved steering inputs. The method imitates the behavior of controllers rather than human inputs, ensuring unbiased data distribution and jitter-free outputs.

## Experiments

- **Data Collection Strategies:** Explored data collection using LIDAR-based obstacle detection, and waypoint-driven scenarios with PID and MPC controllers.

   Data Collected: https://drive.google.com/drive/folders/1_nsHW8zgRbLLXc5W6bpPYwH0OgZFlNOx

- **Fine-Tuning and Optimization:** Experimentation with dropout values, ROI selection, and optimization using the Nadam optimizer to enhance model performance.

## Limitations

- Inpainting Quality drops as resolution of the input image increases.

## Conclusion

This project successfully integrates imitation learning with Model Predictive Control, demonstrating a comprehensive approach to neural network architecture, training, and deployment. Challenges identified provide valuable insights for future exploration. The robustness and adaptability of the model, as well as its real-world limitations, contribute to ongoing research in deep learning for autonomous vehicles.

## Testing Results

### Gradio Demo

[![Click to watch the video](https://img.youtube.com/vi/wiVOA8MBcc4/0.jpg)](https://youtu.be/wiVOA8MBcc4)

### References

1. Airsim: https://github.com/microsoft/AutonomousDrivingCookbook/tree/master/AirSimE2EDeepLearning
2. Model predictive controller: https://github.com/asap-report/carla/tree/racetrack/PythonClient/racetrack 
