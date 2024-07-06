# Drowsiness_detection_shield

## Introduction

### Overview
- Driver drowsiness poses a significant threat to road safety, leading to numerous accidents.
- Our project, the Driver Drowsiness Shield (DDsH), aims to mitigate this risk by employing Transfer Learning and various Machine Learning algorithms.
- We track driver's eye movements via webcam in real-time using OpenCV and Keras. An alarm is triggered if prolonged closure, indicating drowsiness.
- Our proactive approach enhances individual safety and contributes to reducing road accidents, fostering responsible driving.

### Motivations
- Enhancing road safety by addressing the dangers posed by driver drowsiness.
- Mitigating accidents caused by reduced concentration and delayed reactions due to drowsy driving.
- Utilizing advanced technologies like Transfer Learning and computer vision for efficient detection.
- Contributing to societal efforts in reducing road accidents and fatalities.

### Uniqueness of the Work
- Innovative use of Transfer Learning to address class imbalance in models.
- Adapts pre-trained models for enhanced drowsiness detection accuracy.
- Leverages insights from large-scale datasets and related tasks.
- Enhanced performance with reduced need for large labeled datasets.
- Balanced feature representation and data augmentation for reliability.

## Literature Survey

### Existing Systems
- Mercedes-Benz's Attention Assist or Volvo's Driver Alert Control.
- Commercially available wearable devices like the SmartCap or Optalert, which monitor driver fatigue through EEG signals or eyelid movement.
- Research into smartphone applications like SafeDrive or DriveSafe, which use machine learning algorithms to analyze driving behavior and detect signs of drowsiness.
- Studies demonstrating the effectiveness of alerting mechanisms like audible alarms, seat vibrations, or visual warnings in preventing accidents caused by drowsy driving.

### Problem Identification
- Feature Representation and Selection
- Model Training and Generalization
- Class Imbalance and Bias
- Evaluation Metrics and Validation

## Algorithms and Libraries Used

### Libraries
- OpenCV
- numpy
- Tensorflow
- Keras
- Matplotlib

### Algorithms Used
- Transfer Learning
- Haar Cascade Classifier (for detecting eyes)
- Confusion matrix

## Methods and Parameters Used

### Evaluation Measures
- **Accuracy**: \(\text{True Positive} + \text{True Negative} / \text{True Positive} + \text{True Negative} + \text{False Positive} + \text{False Negative}\)
- **Precision**: \(\text{True Positive} / \text{True Positive} + \text{True Negative}\)
- **Recall**: \(\text{True Positive} / \text{True Positive} + \text{False Negative}\)
- **F1 Score**: \(2 \times \frac{\text{Precision} \times \text{Recall}}{\text{Precision} + \text{Recall}}\)

### Parameters

| Parameter                 | Value         |
|---------------------------|---------------|
| Original Image Size       | 84 x 84       |
| Pre Processed Image Size  | 224 x 224     |
| Models                    | MobileNet     |
| Weights                   | Imagenet      |
| Include top               | False         |
| Include tensor            | (224,224,3)   |
| Activation                | Linear        |
| Epochs                    | 5             |
| Optimizer                 | Adam          |
| Loss                      | Mean Squared Error |
| Validation Split          | 0.1           |
| Metrics                   | Accuracy      |

## Experimentation and Results

### System Specifications
- Windows 7 or higher
- i5 processor system or higher
- 8 GB RAM or higher
- 100 GB ROM or higher
- Python (3.6)
- Install IDES (Sublime text Editor / Anaconda / Jupyter Notebook)
- Package of multiple libraries

### Datasets Description
- Dataset are from Google.
- It consists of the following sets:
  - Infrared images (captured in various lighting conditions)
  - High Resolution
  - Low Resolution
- Feature extraction includes:
  - subject ID (37 persons)
  - image ID (84,898 images)
  - glasses presence etc.


#### Calculation
- **Accuracy**: \((5 + 4) / (5 + 4 + 0 + 1) = 0.9\)
- **Precision**: \(5 / (5 + 0) = 1.0\)
- **Recall**: \(5 / (5 + 1) = 0.833\)
- **F1 Score**: \(2 \times \frac{1.0 \times 0.833}{1.0 + 0.833} = 0.909\)

### Conclusion
- Effectively detects drowsiness in real-time, enhancing road safety.
- Utilizes advanced technologies like OpenCV, Tensorflow, and Keras.
- Employs Transfer Learning for reliable detection.
- Contributes to reducing accidents caused by driver fatigue.

### Future Scope
- Implementing advanced algorithms for higher accuracy and efficiency in detecting drowsiness.
- Integrating with vehicle safety systems to enhance overall driver safety seamlessly.
- Utilizing diverse data sources like biometric sensors and environmental data to improve detection robustness.
- Developing real-time monitoring tools that offer enhanced responsiveness and user experience.
- Extending application domains beyond automotive sectors to industries like aviation and heavy machinery.

