README for Collaborative Filtering Algorithm Rating Prediction Project
I. Project Overview
This project aims to use the Singular Value Decomposition (SVD) method in the collaborative filtering algorithm to model and predict user-item rating data. The model's performance is evaluated through 10-fold cross-validation, and rating predictions are made for the test set. Finally, the prediction results are saved as a file.
II. Operating Environment
It is recommended to run the code in the Kaggle Notebook environment to ensure the compatibility of data paths and dependencies.
III. Steps to Run the Code
Prepare the Datasets: Ensure that the training1.txt and testing2.txt dataset files have been uploaded to the /kaggle/input/training/ and /kaggle/input/testing/ directories on Kaggle.
Create and Open a Notebook: Log in to Kaggle, go to the Notebook interface, and click "New Notebook" to create a new Notebook.
Copy and Paste the Code: Copy the project code line by line and paste it into the code cells of the Notebook.
Run the Code: Click the run button (triangle icon) on the left side of each code cell in sequence, or use shortcut keys (such as Shift+Enter) to run the cells. The code will be executed in order, including steps such as data reading, model training, cross-validation evaluation, and test set prediction.
IV. Code Explanation
Environment Check and Dependency Installation: Use !nvidia-smi to check the GPU status; uninstall and reinstall the specified version of numpy through the pip command. However, warnings may occur during the installation process due to dependency conflicts with other packages.
Data Reading and Preprocessing: Use the pandas library to read the training and test set data, adjust the data format, and construct the data objects required by the surprise library.
Model Training and Evaluation: Select the SVD model, set parameters, and use 10-fold cross-validation to evaluate the model's performance. Record the RMSE value for each fold.
Test Set Prediction and Saving: Train the model on the complete training set, make rating predictions for the test set, round the prediction results to two decimal places, and save them as the predictions_final.txt file.
V. Precautions
Ensure that the datasets are correctly uploaded before running the code, and the data format meets the code requirements.
Due to package dependency conflicts, some functions may not run as expected. It is necessary to adjust the versions of the packages according to the actual situation.






