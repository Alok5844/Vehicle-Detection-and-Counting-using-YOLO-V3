# Vehicle-Detection-and-Counting-using-YOLO-V3
## overview
This is a vehicle detection and counting project that aims to count every vehicle(motorcycle, bus, car, cycle, truck, train) in the frame using YOLOv3 object detection algorithm.This type of application can be implemented in traffic system, vehicle paekinf system etc.

## Sample output


https://user-images.githubusercontent.com/35319416/209290662-a3c7c5d8-b8fd-44c1-ac41-b9d18b149a1c.mp4



## YOLOv3 (You Only Look Once - Version 3)
YOLOv3 is a real-time object detection algorithm that recognizes specific objects in images, videos, live streaming.YOLO is a CNN architecture for performing real-time object detection.Version-3 of YOLO was created by Joseph Redmon and Ali Farhadi.The official successor of YOLOv3 is YOLOv4, and the newly released YOLOv7 is been marked as State-of-the-art object detector in 2022.


## Prerequisites
* Linux system(Ubuntu 18.04).
* input video for model.
* Yolov3 pretrained weights.
  create a folder yolo-coco and download the weights in that particular folder.
  
  `mkdir yolo-coco`
  `cd yolo-coco`
  `wget https://pjreddie.com/media/files/yolov3.weights`

## Dependencies for using CPU for computations
* python3 `sudo apt-get upgrade python3`
* pip3 `sudo apt-get install python3-pip`
* OpenCV 3.4 or above `pip3 install opencv-python`
* Imutils `pip3 install imutils`
* Scipy `pip3 install scipy`

## Usage
* `--input` or `-i` argument requires the path to the input video
* `--output` or `-o` argument requires the path to output video
* `--yolo` or `-y` arguments requires the path to the folder where the configuration file, weights and the coco.names file is stored.

format :
  `python3 main.py --input <input_video_path> --output <output_video_path> --yolo yolo-coco`
  
Example :
  `python3 main.py --input /home/proj/yolo/highway_road.mp4 --output /home/proj/yolo/highway_road_out.avi --yolo yolo-coco`
