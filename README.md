# CS-184A-Final-Project

To run this project, we used **Google Colab** for the dependencies
1. Connect to the runtime using a GPU (i.e. T4)
2. On the left sidebar of Colab, click the **Files** icon (folder symbol).
3. Drag and drop the following folders (unzip them) from the submitted zip into the Colab Files area:
      - The `small_dataset` folder
      - The `training_metrics` folder
- Alternatively, you can upload the .zip folders to google colab and run the code snippet to unzip the folders
- If you do **not have** the `small_dataset` folder, then run the small_dataset_generator.ipynb and integrate it into your file structure
- If you do **not have** the `training_metrics` folder, run the train_model.ipynb and integrate it into the file structure
4. Once the upload is complete, run the cells below.
- Additionally, you can edit the model you want to run by following more instructions down below (At section labeled "Download .pth model from Google Drive")

# Project Blocks (project.ipynb)
**Import Data**: We imported a subset of the dataset we used (less than 5 MB) 

**Download .pth model from Google Drive**: Uploaded "fine-tuned" pretrained models to the ipynb file from Google Drive

**Data Preprocessing**: We preprocess the test data only, no training/validation data. We left comments of how the training data is supposed to be transformed

**Instantiate Model, Optimizer, and Loss Function**: Initalize the "fine-tuned" Model and made dummy code for optimizer and loss function (for training)

**Plot Loss/Accuracy Curves**: Plotted the recorded loss and accuracy curves reported in training the "fine-tuned" model

**Evaluate Model on Test Data**: Evaluate model based on small test data

**Compute Accuracy, Precision, Recall, F1 Score, and Confusion Matrix**: Computed the accuracy, precision, recall, F1 score, and Confusion Matrix of the model's performance

# Additional Information
- src contains the models for the iypnb files that we worked on
- small_dataset folder contains only a subset of test data from our dataset
- training_metrics folder contains the loss/accuracy curves for our "fine-tuned" models
- train_model.ipynb fine tunes the pretrained models and records both the model as well as the loss/accuracy curves
- small_dataset_generator.ipynb separates the dataset into a smaller subset for test data
