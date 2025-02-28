Financial Transactions Data Analysis

## Overview
This project focuses on identifying fraudulent financial transactions using machine learning techniques. The dataset contains transaction details such as sender, receiver, transaction amount, date, and transaction type.

## Dataset
The dataset includes the following fields:
- `transaction_id`: Unique identifier for each transaction
- `sender`: Sender of the transaction
- `receiver`: Receiver of the transaction
- `transaction_amount`: Monetary value of the transaction
- `transaction_date`: Date of the transaction
- `transaction_type`: Type of transaction (e.g., deposit, withdrawal)
- `fraud_label`: Indicates if the transaction is fraudulent (1) or non-fraudulent (0)

## Installation
To run this project, install the required dependencies using:

```bash
pip install pandas scikit-learn seaborn matplotlib
```

## Exploratory Data Analysis (EDA)
Performed EDA to identify patterns in transaction amounts, types, and distributions over time. Visualizations include:
- Scatter plots of transaction amounts over years
- Distribution analysis of transactions

## Model Training
We used a `RandomForestClassifier` to classify fraudulent transactions:
1. Preprocessed the dataset by removing unnecessary columns.
2. Split the data into training and testing sets.
3. Trained the model and evaluated its performance using precision, recall, and F1-score.

## Handling Imbalanced Data
Resampling techniques used:
- **Oversampling**: Using `SMOTE` to increase fraudulent transaction samples.
- **Undersampling**: Reducing the number of non-fraudulent transactions.

## Results
The model achieved high accuracy but required balancing due to the dataset being heavily skewed toward non-fraudulent transactions.

## Usage
Run the Jupyter Notebook to:
- Load and preprocess the dataset
- Perform exploratory data analysis
- Train the fraud detection model
- Evaluate model performance

## Contributing
Contributions are welcome! Feel free to fork this repository and submit a pull request.

## License
This project is open-source and available under the MIT License.
