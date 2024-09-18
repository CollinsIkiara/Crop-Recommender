# Crop Recommendation and Revenue Estimates in Agriculture

## Project Title
Machine Learning-Based Crop Recommendation System and Revenue Estimates Analysis

## Project Description
This project leverages machine learning techniques to recommend the most suitable crops for specific soil and environmental conditions. Additionally, it integrates market price analysis to provide farmers with comprehensive insights. By analyzing factors such as soil composition (Nitrogen, Phosphorus, and Potassium levels), environmental parameters (Temperature, Humidity, pH, Rainfall), and current market trends, the system provides data-driven recommendations to farmers, optimizing their decision-making process.


## Installation Instructions
1. Clone this repository:
   ```
   git clone https://github.com/CollinsIkiara/crop-recommendation.git
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
   jupyter notebook 'Crop Recommendation and Revenue Estimates in Agriculture.ipynb'
   ```

## Usage
1. Open the `Crop Recommendation and Revenue Estimates in Agriculture.ipynb` notebook in Jupyter.
2. Run the cells in order to see the data analysis, preprocessing, model training, and evaluation steps.

## Datasets
The datasets used in this project include:
1. **Crop Recommendation Dataset**: This dataset contains various soil parameters such as Nitrogen (N), Phosphorus (P), Potassium (K), and environmental factors (Temperature, Humidity, pH, Rainfall) along with a target crop for the recommendation. (source: [Kaggle](https://www.kaggle.com/datasets/varshitanalluri/crop-recommendation-dataset))
2. **Market Price Dataset**: A dataset containing historical market prices of different crops across various regions. (source: [KAMIS](https://kamis.kilimo.go.ke/site/market))

Both datasets have been preprocessed to ensure high-quality input for the machine learning models.

## Project Workflow
1. **Data Preprocessing**: Cleaning and preparing the datasets for analysis. This includes handling missing values, encoding categorical variables, and scaling numerical values.
2. **Exploratory Data Analysis (EDA)**: Visualizing and understanding the relationships between the features and target variables. This includes identifying correlations and patterns in the data.
3. **Model Building for Crop Recommendation**:
   - Various classification models are tested, including Random Forest, and Logistic Regression.
   - Performance of each model is evaluated using accuracy, precision, recall, and F1-score.
   - Hyperparameter tuning is conducted to improve model performance.
4. **Market Price Analysis**:
   - The predictive models earlier used are reworked to predict revenue estimates using market prices based on historical data.
5. **Model Evaluation**: Final models are selected based on their performance metrics, and recommendations are provided accordingly.

## Results
- The initial model for crop recommendation achieved high accuracy in predicting the most suitable crops based on soil and environmental factors. 
- The final model for the revenue estimate analysis not only achieved high accuracy in predicting the most suitable crops based on soil and environmental factors, but it also provided harvest and revenue estimates, helping farmers make informed decisions about agricultural productivity and profitability.

## Contributors
- [Collins Ikiara](https://github.com/CollinsIkiara)

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Conclusion
This project demonstrates the potential of combining machine learning and data analysis techniques to support farmers in making informed decisions. By providing both crop recommendations and market price forecasts, the system serves as a valuable tool in optimizing agricultural productivity and profitability.

## Future Improvements
1. **Integration of Additional Features**: Including more granular environmental data such as soil moisture and crop disease history to improve the recommendation accuracy.
2. **Real-Time Data**: Incorporating real-time market price data to enhance the revenue forecasting model.
3. **Deployment**: Deploying the model as a web-based application to allow easy access for farmers and agricultural professionals.
