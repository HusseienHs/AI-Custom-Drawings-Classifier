
# Drawing Classifier

The **Drawing Classifier** is an interactive machine learning application that allows users to draw on a canvas, classify their drawings into predefined categories, and train models for prediction. It features a user-friendly GUI, multiple machine learning algorithms, and robust project management capabilities.

---

## Table of Contents

- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [File Structure](#file-structure)
- [Technologies Used](#technologies-used)
- [Screenshots](#screenshots)
- [Future Enhancements](#future-enhancements)
- [Contributing](#contributing)
- [License](#license)

---

## Features

- **Interactive Canvas**:
  - Draw shapes with adjustable brush size.
  - Clear the canvas as needed.

- **Custom Classes**:
  - Define up to three classes for categorizing drawings.

- **Machine Learning**:
  - Train models using saved drawings.
  - Predict the class of new drawings.
  - Switch between various machine learning models, including:
    - Support Vector Machine (SVM)
    - K-Nearest Neighbors (KNN)
    - Logistic Regression
    - Decision Tree
    - Random Forest
    - Gaussian Naive Bayes

- **Project Management**:
  - Save and load projects, including drawings, classes, and trained models.

- **Model Persistence**:
  - Save and load trained models to reuse without retraining.

---

## Requirements

The following tools and libraries are required to run the project:

- **Python**: Version 3.7 or higher
- **Python Libraries**:
  - `numpy`
  - `Pillow`
  - `opencv-python`
  - `scikit-learn`
  - `tkinter` (included with Python)

---

## Installation

Follow these steps to set up and run the Drawing Classifier:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/drawing-classifier.git
   cd drawing-classifier
   ```

2. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the application:
   ```bash
   python drawing_classifier.py
   ```

---

## Usage

### Launch the Application
1. Start the program by running `python drawing_classifier.py`.
2. Enter a project name when prompted:
   - If the project already exists, it will load the saved data.
   - If it’s a new project, define three classes (e.g., "Circle", "Square", "Triangle").

### Drawing and Saving
1. Use the canvas to draw a shape.
2. Save the drawing to one of the three classes using the corresponding button.

### Training the Model
1. Click **"Train Model"** to train the classifier using your saved drawings.

### Prediction
1. Draw a new shape and click **"Predict"** to classify it.

### Model Management
- **Change Model**: Experiment with different machine learning algorithms by clicking "Change Model."
- **Save Model**: Save the trained model to a file for future use.
- **Load Model**: Load a saved model to make predictions.
- **Save Everything**: Save the entire project, including classes, drawings, and the trained model.

---

## File Structure

The application organizes data as follows:

```
project_name/
├── class1/          # Folder for drawings belonging to class 1
│   ├── 1.png
│   ├── 2.png
│   └── ...
├── class2/          # Folder for drawings belonging to class 2
│   ├── 1.png
│   ├── 2.png
│   └── ...
├── class3/          # Folder for drawings belonging to class 3
│   ├── 1.png
│   ├── 2.png
│   └── ...
└── project_name_data.pickle  # Serialized project data
```

---

## Technologies Used

### Programming Language
- Python

### GUI Framework
- `tkinter`

### Image Processing
- `Pillow`
- `opencv-python`

### Machine Learning
- `scikit-learn`

---

## Screenshots

### Main Canvas
_A screenshot of the drawing canvas with buttons for saving, clearing, and adjusting brush size._

### Prediction
_A screenshot showing a prediction popup after classifying a drawing._

---

## Future Enhancements

- **Add More Classes**: Allow users to define more than three classes.
- **Improved Drawing Tools**: Introduce more tools (e.g., straight lines, shapes, eraser).
- **Visualization**: Add a feature to visualize the decision boundaries of the trained models.
- **Performance Metrics**: Show model accuracy and evaluation metrics during training.

---

## Contributing

We welcome contributions to improve this project! To contribute:

1. Fork the repository.
2. Create a feature branch:
   ```bash
   git checkout -b feature/YourFeatureName
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add YourFeatureName"
   ```
4. Push your branch:
   ```bash
   git push origin feature/YourFeatureName
   ```
5. Submit a pull request.

---

## License

This project is licensed under the [MIT License](LICENSE).

---

## Acknowledgments

- Inspired by interactive drawing and classification tools.
- Thanks to contributors and the open-source community for their support.

---

## Contact

For any questions or feedback, feel free to open an issue or contact the repository maintainer.
