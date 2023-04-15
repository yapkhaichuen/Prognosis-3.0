# What is this
This is the primary repository for Prognosis 3.0 clinical CNC skin cancer classifier. 

To start:
```python
pip install -r requirements.txt
```

# Structure
```
├───Local_Run
├───Model_Training
│   └───Skin_Data
│       ├───Cancer
│       │   ├───Testing
│       │   └───Training
│       └───Non_Cancer
│           ├───Testing
│           └───Training
└───Web_App
```
**Local_Run** is almost the same as the Web_App but it runs locally on open-cv with an auto-updating classification pop-up window. 

**Model_Training** trains the model file and saves it in h5 format. DO NOT RUN THIS ON RASPBERRY-PI. To train the model, load the dataset onto Model_Training/Skin_Data. Due to the fact that the dataset is big, please download it separately on Kaggle: https://www.kaggle.com/datasets/kylegraupe/skin-cancer-binary-classification-dataset.

**Web_App** runs a streamlit instance to serve the model for skin-cancer classification. Serves the main use case for Prognosis 3.0.

Most of the sub-applications can be initialised with common python run commands. #ICIA2023
