# Engine Control Unit (ECU) Data Anomaly Detection

This project demonstrates a basic anomaly detection workflow for Engine Control Unit (ECU) data using Python and common data science libraries.

## Project Overview

The goal of this project is to identify unusual patterns or anomalies in simulated ECU data that might indicate potential issues or malfunctions. The workflow involves:

1. **Data Generation:** Simulating ECU data including parameters like RPM, vehicle speed, coolant temperature, throttle position, fuel level, and O2 sensor voltage.
2. **Data Preprocessing:** Scaling the numerical features using `MinMaxScaler` to ensure they contribute equally to the anomaly detection model.
3. **Anomaly Detection:** Applying the Isolation Forest algorithm to identify data points that are significantly different from the majority of the data.
4. **Visualization:** Plotting the vehicle speed data and highlighting the detected anomalies to visually inspect the results.
5. **Anomaly Analysis:** Displaying the data points identified as anomalies.

## Libraries Used

- `pandas`: For data manipulation and analysis.
- `numpy`: For numerical operations and data generation.
- `sklearn`: For data preprocessing (MinMaxScaler) and anomaly detection (IsolationForest).
- `matplotlib`: For data visualization.
- `shap`: For explaining the output of the anomaly detection model (optional, but included in the provided code).

## How to Run

1. Ensure you have the necessary libraries installed (`pip install pandas numpy scikit-learn matplotlib shap`).
2. Run the code cells sequentially in a Python environment (like Google Colab or a Jupyter Notebook).
3. The output will show the head of the generated and scaled dataframes, a plot visualizing the anomalies, and the details of the detected anomalies.

## Potential Extensions

- Explore other anomaly detection algorithms (e.g., Local Outlier Factor, One-Class SVM).
- Implement more sophisticated data preprocessing techniques.
- Integrate with real-world ECU data streams.
- Develop a more interactive visualization dashboard.
- Investigate the root causes of detected anomalies based on domain knowledge.
