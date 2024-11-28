# AI-Training

#Project Results and Overview: Summarize the key objectives, results, and insights from your project. Provide context to help viewers understand the motivation and significance of your work.

At the begining, my projet is a translator opensource with AI on images or vidéos. While it takes a lot of memory to train and I don't have a great computer to do that, I had to reduce at the minimum this project. I will continue this project if I have enough time and the computer for.
The key objectives of this project were : 
  - Using a dataset
  - Training an AI
  - Collecting results

I used google colab to get some VM with GPU and the model YOLOV5 to train my AI. YoloV5 model is a detection model separate in 5 model by the quickest to the more accurate : N, S, M, L, X.

Here is a list of the performance for a 640 pixel image:
        Model	              YAML	        Size          mAPval50-95          Speed CPU ONNX          SpeedA100 TensorRT          params          FLOPs
                                        (pixels)  	       (ms)    	                                        (ms)	                 (M)            (B) 

N     yolov5nu.pt      	yolov5n.yaml	    640	             34.3	                  73.6	                    1.06	                  2.6	          7.7
S     yolov5su.pt	      yolov5s.yaml	    640	             43.0	                  120.7	                    1.27  	                9.1	          24.0
M     yolov5mu.pt      	yolov5m.yaml	    640	             49.0	                  233.9	                    1.86	                  25.1	        64.2
L     yolov5lu.pt      	yolov5l.yaml    	640	             52.2	                  408.4	                    2.50	                  53.2	        135.0
X     yolov5xu.pt      	yolov5x.yaml    	640	             53.2	                  763.2	                    3.81	                  97.2	        246.4

(List from the site : https://docs.ultralytics.com/fr/models/yolov5/#performance-metrics ) 

First, I train the AI to analyze and find the letters in a lor of images. My dataset for the training is a dataset opensource on RoboFlow with 1175 images with label:  https://universe.roboflow.com/ann36chen-hbcoz/0603-3/dataset/7
To compare, I used YoloV5 S, M, L and X. Every train with every model was more and more accurate.

#Source Code: Organize and document all source code for the project. Include a clear file structure, instructions for setup, and any necessary dependencies for running the code.

#Performance Metrics: Detail the performance metrics achieved by your project, including accuracy, speed, memory efficiency, or any other relevant benchmarks. Consider using graphs or tables for better clarity.

#Installation and Usage: Provide step-by-step instructions for installing and running the project. Include examples or scripts to demonstrate typical usage.

#References and Documentation: Link to any relevant papers, libraries, or other sources that contributed to your project. Include explanations of key algorithms or techniques as needed.

#Issues and Contributions: Specify any known issues or limitations, and encourage contributions by outlining how others can contribute, report bugs, or suggest enhancements.

#Future Work: Briefly discuss any potential improvements or areas for future development to show the direction of your work.
