Sure! Here are three `README.md` files for the different scripts you provided:

**1. detect_mask_image.py**

```markdown
# Detect Mask in an Image

This script allows you to detect face masks in an image. It utilizes a pre-trained deep learning model to detect faces and another model to classify whether the detected faces are wearing masks or not.

## Usage

1. Install the required packages mentioned in the `requirements.txt` file.
2. Run the script using the following command:

   ```shell
   python detect_mask_image.py --image <path_to_image>
   ```

   Replace `<path_to_image>` with the path to the input image.

## Dependencies

- tensorflow
- opencv-python
- imutils
- numpy

## Models

- Face Detector Model: The script uses a pre-trained face detector model provided in the `face_detector` directory.
- Face Mask Detector Model: The script loads a pre-trained face mask detector model from the file `mask_detector.model`.

Feel free to experiment with different images to detect face masks.
```

**2. detect_mask_video.py**

```markdown
# Real-time Face Mask Detection in Video

This script performs real-time face mask detection in a video stream. It uses a webcam or any other video source to capture frames, detects faces in each frame, and predicts whether the detected faces are wearing masks or not.

## Usage

1. Install the required packages mentioned in the `requirements.txt` file.
2. Run the script using the following command:

   ```shell
   python detect_mask_video.py
   ```

   The script will open a new window showing the video stream with face mask detection.

3. Press the 'q' key to stop the video stream and close the window.

## Dependencies

- tensorflow
- opencv-python
- imutils
- numpy

## Models

- Face Detector Model: The script uses a pre-trained face detector model provided in the `face_detector` directory.
- Face Mask Detector Model: The script loads a pre-trained face mask detector model from the file `mask_detector.model`.

Enjoy real-time face mask detection in videos!
```

**3. train_mask_detector.py**

```markdown
# Train Face Mask Detector

This script trains a face mask detector using a dataset of images. It uses transfer learning with the MobileNetV2 architecture to train the model.

## Usage

1. Prepare your dataset by organizing it into two categories: `with_mask` and `without_mask`. Place the images in the corresponding directories.
2. Install the required packages mentioned in the `requirements.txt` file.
3. Run the script using the following command:

   ```shell
   python train_mask_detector.py
   ```

   The script will read the dataset, split it into training and testing sets, and train the face mask detector model.

4. After training, the script will display the classification report showing the accuracy and other metrics of the trained model.

## Dependencies

- tensorflow
- opencv-python
- imutils
- numpy
- scikit-learn
- matplotlib

## Dataset Structure

The dataset directory should follow this structure:

```
dataset/
    ├── with_mask/
    │   ├── image1.jpg
    │   ├── image2.jpg
    │   └── ...
    └── without_mask/
        ├── image1.jpg
        ├── image2.jpg
        └── ...
```

The trained face mask detector model will be saved as `mask_detector.model`.
