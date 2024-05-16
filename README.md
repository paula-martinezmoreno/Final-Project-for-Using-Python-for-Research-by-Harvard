# Final-Project-for-Using-Python-for-Research-by-Harvard
This repository contains my final project for the "Using Python for Research" course offered by Harvard University. The course provided a comprehensive introduction to using Python for scientific research, covering topics such as data analysis, statistical methods, and visualization techniques.

The project focuses on predicting the type of physical activity (e.g., walking, climbing stairs) using tri-axial smartphone accelerometer data. Different physical activities generate distinct patterns of acceleration, which can be analyzed to classify the activity accurately.

## Project Instructions

The project involves the following steps:

1. **Input Data**:
   - **train_time_series.csv**: Contains raw accelerometer data collected using the Beiwe research platform.
     - Format: `timestamp, UTC time, accuracy, x, y, z`
     - We use the `timestamp` column as the time variable and the `x`, `y`, and `z` columns for measurements of linear acceleration.
   - **train_labels.csv**: Contains activity labels with the following encoding:
     - `1 = standing`, `2 = walking`, `3 = stairs down`, `4 = stairs up`
     - Labels are provided for every 10th observation in `train_time_series.csv`.

2. **Goal**:
   - Classify different physical activities as accurately as possible.
   - Test the accuracy of the classification model using `test_time_series.csv` and provide predicted activity labels.

3. **Output**:
   - A CSV file named `test_labels.csv` containing the timestamps and corresponding class predictions (1, 2, 3, 4).

4. **Performance Measurement**:
   - Measure and report the running time of the code from loading the test data to computing the predictions.

## Technologies Used

- Python
- NumPy
- Pandas
- Scikit-Learn
- Matplotlib
- Jupyter Notebook

## Repository Contents

- `final_project.py`: Main script implementing the research project.
- `train_time_series.csv`: Raw accelerometer data for training.
- `train_labels.csv`: Activity labels for training.
- `test_time_series.csv`: Raw accelerometer data for testing.
- `test_labels.csv`: Template for the test labels output.
- `final_project_notebook.ipynb`: Jupyter notebook with detailed analysis, visualizations, and explanations of the research.
- `README.md`: This file with project details.

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/final-project-using-python-for-research.git
