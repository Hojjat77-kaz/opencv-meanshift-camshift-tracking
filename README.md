# Object Tracking with MeanShift and CamShift

A computer vision project that demonstrates object tracking using the MeanShift and CamShift algorithms in OpenCV.

## Features

* ROI (Region of Interest) selection
* HSV color space conversion
* Histogram-based object representation
* Histogram normalization
* Histogram Back Projection
* MeanShift object tracking
* CamShift object tracking
* Real-time video tracking visualization
* Comparison between MeanShift and CamShift

## Technologies Used

* Python
* OpenCV
* NumPy

## Algorithms

### MeanShift

MeanShift tracks an object by locating the region with the highest probability density based on the object's color histogram.

Characteristics:

* Tracks object position
* Fixed tracking window size
* Fast and lightweight
* Suitable for simple tracking tasks

### CamShift

CamShift (Continuously Adaptive Mean Shift) extends MeanShift by adapting the tracking window size and orientation.

Characteristics:

* Tracks object position
* Updates window size automatically
* Handles scale changes
* Estimates object rotation
* More robust than MeanShift

## Processing Pipeline

1. Read video frame
2. Select initial ROI
3. Convert ROI to HSV
4. Compute object histogram
5. Normalize histogram
6. Generate Back Projection map
7. Apply MeanShift or CamShift
8. Update tracking window
9. Draw tracking result
10. Display output

## Concepts Practiced

* Object Tracking
* HSV Color Space
* Histogram Analysis
* Histogram Normalization
* Back Projection
* MeanShift Algorithm
* CamShift Algorithm
* Motion Tracking
* Video Processing

## MeanShift Workflow

ROI

↓

Histogram

↓

Back Projection

↓

MeanShift

↓

Updated Window Position

## CamShift Workflow

ROI

↓

Histogram

↓

Back Projection

↓

CamShift

↓

Updated Position + Size + Rotation

## Example Output

Tracking Window Detected

Object Position Updated

Object Successfully Tracked Across Frames

## MeanShift vs CamShift

| Feature             | MeanShift | CamShift        |
| ------------------- | --------- | --------------- |
| Position Tracking   | Yes       | Yes             |
| Adaptive Size       | No        | Yes             |
| Rotation Estimation | No        | Yes             |
| Speed               | Faster    | Slightly Slower |
| Robustness          | Moderate  | Higher          |

## Future Improvements

* Multi-object tracking
* Kalman Filter integration
* SORT tracking algorithm
* Deep Learning based trackers
* Real-time webcam tracking
* Object re-identification

## What I Learned

This project helped me understand:

* How object tracking differs from object detection
* How histograms represent object appearance
* How Back Projection creates probability maps
* How MeanShift searches for the highest density region
* How CamShift adapts to object scale and rotation
* How classical tracking algorithms work in computer vision
