# SMS Spam Detection System using Deep Learning in TensorFlow2

<p align="center">
  <img src="images/spam_sms_image_01.png" width="900">
</p>


## 🚀 Project Overview

This project is about building a Spam Detection System for SMS messages using deep learning techniques in TensorFlow2 and NLP.<br>
Three different architectures namely Dense Network, LSTM, and Bi-LSTM have been used to build the spam detection model.<br>
The accuracy of the models is compared and evaluated to select the best one.<br>
<br>


## 📂 Folder Structure
```

/
├── app/
│   └── app.py
├── data/
│   └── SMSSpamCollection.txt
├── images
│   └── spam_sms_image_01.png
├── models
│   └── Bi-LSTM_spam_detection.h5
│   └── Dense_Spam_Detection.h5
│   └── LSTM_Spam_Detection.h5
├── notebooks
│   └── sms-spam-detection-nlp.ipynb
├── .gitignore
├── README.md
└── requirements.txt

```
<br>

### Steps Involved :
The following steps are involved in the project:<br>

1. Load and Explore the Data: The dataset is loaded into a Pandas DataFrame and explored to get insights into the distribution of ham and spam messages.<br>

2. Prepare Train-Test Data: The messages are tokenized, and their corresponding labels are one-hot encoded. The dataset is split into training and testing sets in the ratio of 80:20.<br>

3. Train the Spam Detection Model: The three models - Dense Network, LSTM, and Bi-LSTM - are trained using the training dataset. The models are evaluated using the validation dataset.<br>

4. Compare and Select the Final Model: The accuracy of the models is compared, and the best-performing model is selected.<br>

5. Use the Final Trained Classifier to Classify New Messages: The final model is used to classify new messages as ham or spam.<br>



### Accuracy of the Models :
The accuracy of the models is as follows: <br>

Dense Network - 98.5%<br>
SVM - 97.6%<br>
Bi-LSTM - 98.8%<br>
LSTM - 98.6%<br>



# Create & activate virtual environment
python -m venv venv

# Windows
venv\Scripts\activate

# macOS / Linux
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Run Streamlit app
streamlit run app.py



















