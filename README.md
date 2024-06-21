# 💤 Drowsiness Detection Using YOLOv7 🚙

## Overview
This project utilizes the YOLOv7 architecture to develop a drowsiness detection system. The model is designed to identify signs of driver drowsiness, such as closed eyes, yawning, and head movements, using a custom dataset. However, the results indicate that YOLOv7 may not be the best choice for real-time drowsiness detection.

## Performance Analysis
### Quantitative Results
The YOLOv7 model was trained and tested over 25 epochs, yielding the following results:

- **Mean Average Precision (mAP)**: 0.95970 for the training dataset after 25 epochs.
- **Training Precision**: 0.91640
- **Training Recall**: 0.93820

### Qualitative Results

## Model Performance Metrics
| Algorithm | Accuracy | Precision | Recall | F1 Score | Missing Detection Score | Inference Time (seconds) |
|-----------|----------|-----------|--------|----------|-------------------------|--------------------------|
| **YOLOv7**    | 0.19047  | 0.33333   | 0.06250| 0.10526  | 0.04762                 | 202.21893                |

## Results
<table>
  <tr>
    <td style="text-align: center;">
      <img src="https://github.com/ParthJohri/Drowsiness_Detection_Using_YOLOv7/blob/main/results/F1_curve.png" alt="F1 Curve" style="width: 400px;">
      <br>F1 Curve
    </td>
    <td style="text-align: center;">
      <img src="https://github.com/ParthJohri/Drowsiness_Detection_Using_YOLOv7/blob/main/results/PR_curve.png" alt="PR Curve" style="width: 400px;">
      <br>PR Curve
    </td>
    <td style="text-align: center;">
      <img src="https://github.com/ParthJohri/Drowsiness_Detection_Using_YOLOv7/blob/main/results/P_curve.png" alt="Precision Curve" style="width: 400px;">
      <br>Precision Curve
    </td>
  </tr>
  <tr>
    <td style="text-align: center;">
      <img src="https://github.com/ParthJohri/Drowsiness_Detection_Using_YOLOv7/blob/main/results/R_curve.png" alt="Recall Curve" style="width: 400px;">
      <br>Recall Curve
    </td>
    <td style="text-align: center;">
      <img src="https://github.com/ParthJohri/Drowsiness_Detection_Using_YOLOv7/blob/main/results/confusion_matrix.png" alt="Confusion Matrix" style="width: 400px;">
      <br>Confusion Matrix
    </td>
    <td style="text-align: center;">
      <img src="https://github.com/ParthJohri/Drowsiness_Detection_Using_YOLOv7/blob/main/results/results.png" alt="Results" style="width: 400px;">
      <br>Results
    </td>
  </tr>
</table>

These results suggest that YOLOv7 is not suitable for real-time drowsiness detection due to its low accuracy and high inference time.

## Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/ParthJohri/Drowsiness_Detection_Using_YOLOv7.git
   ```
2. Navigate to the project directory:
   ```sh
   cd Drowsiness_Detection_Using_YOLOv7
   ```
3. Install the required packages:
   ```sh
   pip install -r requirements.txt
   ```

## Usage
1. Prepare your dataset with labeled images for training and testing.
2. Train the YOLOv7 model using the provided training script.
3. Test the model on the test dataset to evaluate its performance.
4. Due to the model's low accuracy and high inference time, consider alternative YOLO versions or different architectures for real-time driver monitoring.

## Future Work
- **Model Optimization**: Investigate ways to improve YOLOv7's accuracy and reduce inference time.
- **Dataset Expansion**: Include more diverse datasets to improve model robustness and generalization.
- **Alternative Models**: Explore other YOLO versions or different architectures better suited for real-time implementation.

## Contributing
Contributions to improve the drowsiness detection system are welcome. Please fork the repository, make your changes, and submit a pull request.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
