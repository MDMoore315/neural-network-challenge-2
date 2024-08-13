# neural-network-challenge-2

### Overview

The purpose of this project is to develop a machine learning model that Human Resources can use to help predict employee attrition and department assignment multiple parameters. These include Age, Job Involvement, Job Satisfaction, Distance From Home, Years In Current Role, Years Since Last Promotion, Work Life Balance, Overtime, Job Role and Training Times Last Year. Following the standard process we move through data preprocessing, neural network creation, model training and performance evaluation. The intent here is to allow companies to better understand their employees and identify strategies to improve employee retention, as well as identify the best department for individual employees.

### Functionality

1. **Preprocessing** includes: 
   - **Data Import and Cleaning**: Importing the data, determining unique values
   - **Dataframe Creation**: Creating the 'y' dataframe based on the attrition and department columns. Also, created the 'x' dataframe based on selected columns
   - **train_test_split**: Splits the data into training and testing data.
   - **StandardScaler**: Standardizes and scales features.
   - **pd.get_dummies**: Converts categorical variables.
   - **OneHotEncoder**: Encodes the two categorical columns into a suitable format.

2. **Neural Network Creation**:
   - **Input Layer**: Accepts the preprocessed feature set.
   - **Shared Layers**: Adds two shared layers (64 and 32 neurons) with the ReLU activation function.
   - **Department Branch**:
     - **Hidden Layer**: A dense layer with 16 neurons and ReLU activation function.
     - **Output Layer**: A dense layer with softmax activation to predict the department.
   - **Attrition Branch**:
     - **Hidden Layer**: A dense layer with 16 neurons and ReLU activation function.
     - **Output Layer**: A dense layer with softmax activation to predict attrition status.

3. **Training and Evaluation**:
   - **Create the model
   - **model.compile**: Compiles the model with the Adam optimizer and categorical cross-entropy loss for both department and attrition.
   - **model.fit**: Fits the model on the training data for 100 epochs.
   - **model.evaluate**: Evaluates the model's performance on the test data.
   - **Accuracy Calculation**: Calculates and displays the accuracy for both department and attrition predictions.


GitHub Copilot, ChatGPT, and/or Bootcamp Module Activity files were used for guidance and debugging purposes.
