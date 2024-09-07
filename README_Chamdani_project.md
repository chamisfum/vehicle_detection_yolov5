# Vehicle Detection with YOLOv5

Welcome to the **Vehicle Detection** project! This project uses YOLOv5 to detect various types of vehicles in videos. YOLOv5 is a state-of-the-art object detection model that provides high accuracy and speed.

## Overview

In this project, we leverage YOLOv5 to detect vehicles such as cars, buses, and trucks in high-resolution videos. The model is run with specific parameters to ensure optimal performance for vehicle detection.

## Getting Started

### Prerequisites

Before running the detection script, ensure you have the following:

- Python 3.6 or later
- YOLOv5 repository cloned
- Required Python packages installed

### Installation

1. **Clone YOLOv5 Repository**

   If you haven't already, clone the YOLOv5 repository from GitHub:
   ```bash
   git clone https://github.com/ultralytics/yolov5
   cd yolov5
   ```

2. **Install Dependencies**

   Install the necessary Python packages:
   ```bash
   pip install -r requirements.txt
   ```

3. **Download YOLOv5 Weights**

   Ensure you have the YOLOv5 weights file `yolov5s.pt`. You can download it from the YOLOv5 [release page](https://github.com/ultralytics/yolov5/releases).

### Running Vehicle Detection

To run the vehicle detection script, use the following command:

```bash
python detect.py --weights yolov5s.pt --source video_1440p.mp4 --conf 0.4 --img-size 640 --classes 2 5 7
```

#### Parameters:
- `--weights yolov5s.pt`: Specifies the YOLOv5 model weights. In this case, `yolov5s.pt` is the small version of YOLOv5, which balances speed and accuracy.
- `--source video_1440p.mp4`: Path to the input video file. Ensure the video is in 1440p resolution for best results.
- `--conf 0.4`: Confidence threshold for detections. The model will only show detections with confidence scores above 40%.
- `--img-size 640`: Size of the images used for detection. A value of 640 is recommended for a good balance between speed and accuracy.
- `--classes 2 5 7`: Class indices to detect:
  - `2` - Car
  - `5` - Bus
  - `7` - Truck

### Output

The output video will be saved in a folder named `runs/detect/exp`. It will show the detected vehicles with bounding boxes and class labels.

### Example

Here's an example of the command in action:

```bash
python detect.py --weights yolov5s.pt --source video_1440p.mp4 --conf 0.4 --img-size 640 --classes 2 5 7
```

This command will process `video_1440p.mp4`, detect vehicles (cars, buses, and trucks) with a confidence threshold of 40%, and save the results.

## Troubleshooting

- **Error: 'ModuleNotFoundError'** - Ensure all dependencies are installed using `pip install -r requirements.txt`.
- **No detections** - Check if the input video is in the correct format and resolution.

## Contact Information

For further questions or assistance, you can reach out to:

- **Name**: Moch. Chamdani Mustaqim
- **Phone**: +6285655746306
- **GitHub**: [chamisfum](https://github.com/chamisfum)
- **LinkedIn**: [moch-chamdani-mustaqim](https://www.linkedin.com/in/moch-chamdani-mustaqim/)
- **CV**: [View CV](https://drive.google.com/file/d/1qAy49ysZajfbJZ7SraTpG8rYPNsvKa8D/view?usp=sharing)
- **Assignment Project**: [View Assignment Project](https://github.com/chamisfum/vehicle_detection_yolov5)

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- **YOLOv5**: Thanks to the YOLOv5 team for their incredible work on the model.
- **Ultralytics**: For providing the YOLOv5 repository and pre-trained models.

---