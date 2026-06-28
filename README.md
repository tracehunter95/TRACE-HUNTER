##### TRACE-HUNTER #####

# DEEP Learning Projects
This repository contains deep learning notebooks created in Google Colab.

## Projects :

### Network Traffic & Website Classifier (`BE_PROJECT.ipynb`)
A dual-purpose deep learning model designed to analyze sequences of network packets. The model simultaneously performs two tasks:
* Website Classification: Identifies which of 34 specific websites (e.g., Google, Amazon, Netflix) the network traffic belongs to.
* Intrusion Detection: Classifies the traffic flow as either `normal` or a synthetic `attack`.

## Key Features:
* *Architecture: Multi-task neural network utilizing a "CNN-BiLSTM-Attention" structure.
* *'1D-CNN' for extracting spatial features from packet sequences.
* *'Bidirectional LSTM' for learning the temporal dependencies of the network flow.
* *'Custom Attention Layers' to weigh the importance of specific packets within the sequence.
* *Data Engineering: Extracts features such as packet length, flow direction, and inter-arrival time. Synthesizes attack data by introducing jitter and dummy padding to normal packet timestamps and sizes. 
* *Performance: Achieved ~96% accuracy for attack detection and ~90% accuracy for website classification on the test dataset.
* *User Interface: Includes a built-in Streamlit web interface for users to upload sequences and get real-time classification predictions.

## Tools :
* *Languages & Environments: Python, Google Colab, Jupyter Notebook
* *Deep Learning Framework: TensorFlow / Keras
* *Data Processing: Pandas, NumPy, Scikit-Learn (MinMaxScaler)
* *Deployment / GUI: Streamlit
