# Bank Note Authentication using StreamLit:

• StreamLit is used to build beautiful custom web-apps for machine learning and data science.

|Language Used: | Python             |
|---------------|--------------------|

|IDE 1 Used:    | Jupyter Notebook |
|---------------|--------------------|

|IDE 2 Used:    | PyCharm          |
|---------------|--------------------|

## Get the Dataset:

Data were extracted from images that were taken from genuine and forged banknote like specimens. For digitization, an industrial camera was used for print inspection. The final images have 400x400 pixels. Due to the object lens and distance to the investigated object gray-scale pictures with a resolution of about 600 dpi were gained. Wavelet Transform tool were used to extract features from images. Dataset was retrieved from UCI Repositories.

Extracted Features = Variance, Skewness, Curtosis, Entropy and Class

Where;

class 0 => Fake / Inauthentic

class 1 => Authentic

## Import the Dataset:

The name of the dataset I have used for this project is 'BankNoteAuthentication.csv'.

Dataset contains five columns -> Variance, Skewness, Curtosis, Entropy and Class. The shape of our dataset is (1373, 5).

In BankNoteAuthentication.csv, first four columns i.e. Variance, Skewness, Curtosis, Entropy are independent variables whereas fifth column Class is dependent variable.

## Essential Libraries:

Following are the essential libraries which need to be imported

• Pandas

• Numpy

• Matplotlib

• Scikit-Learn

• Scipy

• Pickle

• PIL

• StreamLit

## Matrix of Dependent and Independent Variables:

In Python, you have to create two matrices for independent variables and dependent variable.

Hence for BankNoteAuthentication.csv, create one matrix for four independent variables and then create one matrix dependent variable.

## Split the Dataset into Training Data and Test Data:

ML is about a machine that is going to learn from the data to make predictions.

We need to split the dataset into training set and test set. Using training set, we build the machine learning model and using test set, we test the performance of this machine learning model.

We are building our ML model on training set by establishing some correlation between independent variables and dependent variables and once the ML model understands the correlation between independent variables and dependent variables. We will test if the ML model can apply the correlations you understood based on training set on test set.

In brief, we have to make two different datasets. The training set on which the machine learning model learns and test set on which we test if the ML model learned correctly the correlations.

In Python, model_selection class from scikitlearn library is used to split the dataset into training and test set.

In this project, I have given 70% of data for training and 30% of data for testing.

## Applying Random Forest Classifier:

Random forests are an ensemble learning method for classification, regression and other tasks that operate by constructing a multitude of decision trees at training time and outputting the class that is the mode of the classes or mean prediction of the individual trees.

## Accuracy Score:
In this project I have achieved an accuracy of 99% (0.9902912621359223)

## Creating Pickle File:
After creating classifier model we need to create a pickle file, so that it can be used in flask app. This can be done using Serialization.

## Create Web Page using StreamLit Library: (File Name => StreamLitApp.py)

Step 1: Open and Load Pickle File.

Step 2: This will be running at localhost:8501

Step 3: Create Web Page / App for Prediction.

Step 4: Command => streamlit run StreamLitApp.py

## Thank you for visiting my GitHub repository!

# Contact Information:

If you have any questions, suggestions, or would like to connect, feel free to reach out to me:

• Mobile Number: UAE => +971-562205977 / India => +91-9820989602

• Email: analyst.asadqadri@gmail.com

• LinkedIn: https://www.linkedin.com/in/asadqadri/

• GitHub: https://github.com/asadqadri

• Tableau Public: https://public.tableau.com/profile/asad.qadri

Looking forward to engaging with fellow data enthusiasts and industry professionals! 😊
