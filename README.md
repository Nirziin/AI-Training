# AI-Training

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)

## Project Results and Overview: 
Summarize the key objectives, results, and insights from your project. Provide context to help viewers understand the motivation and significance of your work.

<a href="https://docs.ultralytics.com/models/yolo11/" target="_blank">
  <img width="100%" src="https://raw.githubusercontent.com/ultralytics/assets/refs/heads/main/yolo/performance-comparison.png" alt="YOLO11 performance plots">
</a>

At the begining, my projet is a translator opensource with AI on images or vidéos. While it takes a lot of memory to train and I don't have a great computer to do that, I had to reduce at the minimum this project. I will continue this project if I have enough time and the computer for.
The key objectives of this project were : 
  - Using a dataset
  - Training an AI
  - Collecting results

I used google colab to get some VM with GPU and the model YOLOV5 to train my AI. YoloV5 model is a detection model separate in 5 model by the quickest to the more accurate : N, S, M, L, X.

Here is a list of the performance for a 640 pixel image:
| Model                                                                                           | size<br><sup>(pixels) | mAP<sup>val<br>50-95 | mAP<sup>val<br>50 | Speed<br><sup>CPU b1<br>(ms) | Speed<br><sup>V100 b1<br>(ms) | Speed<br><sup>V100 b32<br>(ms) | params<br><sup>(M) | FLOPs<br><sup>@640 (B) |
| ----------------------------------------------------------------------------------------------- | --------------------- | -------------------- | ----------------- | ---------------------------- | ----------------------------- | ------------------------------ | ------------------ | ---------------------- |
| [YOLOv5n](https://github.com/ultralytics/yolov5/releases/download/v7.0/yolov5n.pt)              | 640                   | 28.0                 | 45.7              | **45**                       | **6.3**                       | **0.6**                        | **1.9**            | **4.5**                |
| [YOLOv5s](https://github.com/ultralytics/yolov5/releases/download/v7.0/yolov5s.pt)              | 640                   | 37.4                 | 56.8              | 98                           | 6.4                           | 0.9                            | 7.2                | 16.5                   |
| [YOLOv5m](https://github.com/ultralytics/yolov5/releases/download/v7.0/yolov5m.pt)              | 640                   | 45.4                 | 64.1              | 224                          | 8.2                           | 1.7                            | 21.2               | 49.0                   |
| [YOLOv5l](https://github.com/ultralytics/yolov5/releases/download/v7.0/yolov5l.pt)              | 640                   | 49.0                 | 67.3              | 430                          | 10.1                          | 2.7                            | 46.5               | 109.1                  |
| [YOLOv5x](https://github.com/ultralytics/yolov5/releases/download/v7.0/yolov5x.pt)              | 640                   | 50.7                 | 68.9              | 766                          | 12.1                          | 4.8                            | 86.7               | 205.7                  |

[List from this site](https://docs.ultralytics.com/fr/models/yolov5/#performance-metrics)

First, I train the AI to analyze and find the letters in a lor of images. 
  - [My dataset](https://universe.roboflow.com/ann36chen-hbcoz/0603-3/dataset/7) for the training is a dataset opensource on RoboFlow with 1175 images with label.
To compare, I used YoloV5 S, M, L and X. Every train with every model was more and more accurate.

## Source Code: 
Organize and document all source code for the project. Include a clear file structure, instructions for setup, and any necessary dependencies for running the code.

## Performance Metrics: 
Detail the performance metrics achieved by your project, including accuracy, speed, memory efficiency, or any other relevant benchmarks. Consider using graphs or tables for better clarity.

## Installation and Usage:
Provide step-by-step instructions for installing and running the project. Include examples or scripts to demonstrate typical usage.

## References and Documentation: 
Link to any relevant papers, libraries, or other sources that contributed to your project. Include explanations of key algorithms or techniques as needed.

## Issues and Contributions: 
Specify any known issues or limitations, and encourage contributions by outlining how others can contribute, report bugs, or suggest enhancements.

## Future Work: 
Briefly discuss any potential improvements or areas for future development to show the direction of your work.
