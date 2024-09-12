# Crop Recommendation in Agriculture

## Project Title
Machine Learning-Based Crop Recommendation System

## Project Description
This project leverages machine learning techniques to recommend the most suitable crops for specific soil and environmental conditions. By analyzing factors such as soil composition (Nitrogen, Phosphorus, and Potassium levels) and environmental parameters (Temperature, Humidity, pH, Rainfall), the system provides data-driven suggestions to farmers and agricultural professionals. The goal is to optimize crop selection, enhance yield, and promote sustainable farming practices.

## Installation Instructions
1. Clone this repository:
   ```
   git clone https://github.com/yourusername/crop-recommendation.git
   cd crop-recommendation
   ```
2. Create a virtual environment (optional but recommended):
   ```
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```
3. Install required libraries:
   ```
   pip install -r requirements.txt
   ```
4. Launch Jupyter Notebook:
   ```
   jupyter notebook
   ```

## Usage
1. Open the `Crop Recommendation In Agriculture.ipynb` notebook in Jupyter.
2. Run the cells in order to see the data analysis, preprocessing, model training, and evaluation steps.
3. To make predictions with the trained model:
   ```python
   # Example usage (replace with actual values)
   input_data = [[90, 40, 40, 20, 80, 7, 200]]  # N, P, K, temperature, humidity, ph, rainfall
   prediction = model.predict(input_data)
   print(f"Recommended crop: {prediction[0]}")
   ```

## Data
- **Dataset**: Crop recommendation dataset (source: [Kaggle](https://www.kaggle.com/datasets/varshitanalluri/crop-recommendation-dataset))
- **Features**: N (Nitrogen), P (Phosphorus), K (Potassium), temperature, humidity, pH, rainfall
- **Target**: Crop (22 different crops)
- **Preprocessing**: Numerical features were scaled using StandardScaler, and the target variable was encoded using LabelEncoder.

## Methodology
1. **Data Analysis**: Explored the dataset structure, checked for missing values, and visualized feature relationships.
2. **Data Preprocessing**: Scaled numerical features and encoded the target variable.
3. **Model Selection**: Experimented with various classification algorithms (e.g., Random Forest, Logistic Regression) and performed hyperparameter tuning.
4. **Model Evaluation**: Assessed model performance using metrics such as accuracy, precision, recall, and F1-score.

## Results
- The Random Forest Classifier achieved the highest accuracy of 99.3% on the test set. Upon cross-validation, it improved to 99.5%
- Key features influencing crop recommendations: Potassium content, Humidity, and Phosphorus content.
- The model successfully differentiates between crops with similar growing conditions.

## Contributors
- [Collins Ikiara](https://github.com/CollinsIkiara)

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Conclusion
This machine learning-based crop recommendation system demonstrates the potential of data-driven decision-making in agriculture. By providing accurate crop suggestions based on specific field conditions, it can help farmers optimize their crop selection, potentially leading to improved yields and more sustainable farming practices. Future work could involve incorporating additional environmental factors, expanding the dataset, or developing a user-friendly interface for easier adoption by agricultural professionals.
