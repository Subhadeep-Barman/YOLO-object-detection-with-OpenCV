Absolutely! Here’s the revised version with updated categories:

---

### YOLO Object Detection with OpenCV

**Object Detection Using YOLO and OpenCV**

This project showcases object detection in both images and video streams using YOLOv3 and OpenCV with Python. The YOLO model employed here is pre-trained on the COCO dataset.

The COCO dataset includes 80 categories such as:

- Persons
- Motorcycles
- Buses and trucks
- Helicopters
- Fire extinguishers and traffic cones
- Wildlife (e.g., lions, bears, elephants)
- Household items (e.g., lamps, tables, refrigerators)
- And much more!


**YOLOv3 Pre-trained Model:**

- **Model Files**: YOLOv3 pre-trained on the COCO dataset, created by the Darknet team.

**Object Detection in Images with YOLO:**

**Setup:**

```bash
pip install numpy
pip install opencv-python
```

**Run the Project:**

```bash
python yolo.py --image images/baggage_claim.jpg
```

**Screenshots:**

- YOLO effectively detects people and suitcases in the image, including identifying the handbag on the woman’s shoulder.

- YOLO also identifies players and the soccer ball on the field, even spotting a partially obscured person in the background.

**Object Detection in Video Streams with YOLO:**

**Setup:**

```bash
pip install numpy
pip install opencv-python
```

**Run the Project:**

```bash
python yolo_video.py --input videos/airport.mp4 --output output/airport_output.avi --yolo yolo-coco
```

**Screenshots:**

- The video/GIF demonstrates YOLO’s capability to detect vehicles, people, and traffic lights.
https://github.com/user-attachments/assets/9f87ec7a-8803-48ad-b61a-d5a74700570f

**Limitations:**

One notable limitation of YOLO is:

- **Small Object Detection**: YOLO may struggle with detecting small or closely packed objects due to its grid-based approach. Each grid cell predicts only one object, leading to missed detections if multiple small objects overlap in a single cell.

For better handling of small or clustered objects, consider alternatives like Faster R-CNN (which is slower) or SSDs, which offer a good balance between speed and accuracy.

**Real-Time Object Detection with YOLO and OpenCV:**

**Setup:**

```bash
pip install numpy
pip install opencv-python
pip install imutils
```

**Run the Project:**

```bash
python real_time_object_detection.py
```

**Screenshots:**

- The real-time object detector can identify people, sofas, and chairs effectively.

Feel free to follow and ⭐ my repository!

---
