# IMDB Sentiment Analysis using Simple RNN

This project is a deep learning-based sentiment analysis application that classifies IMDB movie reviews as **Positive** or **Negative**. It uses a **Simple Recurrent Neural Network (Simple RNN)** built with TensorFlow/Keras and provides an interactive **Streamlit web app** for real-time prediction.

## Project Overview

The goal of this project is to understand how Recurrent Neural Networks can be used for Natural Language Processing tasks such as sentiment classification. The model is trained on the IMDB movie review dataset and predicts whether a given review expresses positive or negative sentiment.

## Features

* Preprocesses IMDB text reviews using word indexing and padding
* Builds a Simple RNN model for binary sentiment classification
* Saves and loads a trained `.h5` model
* Provides a Streamlit interface for user input
* Predicts sentiment score and final sentiment label
* Includes Jupyter notebooks for training, embedding, and prediction

## Tech Stack

* Python
* TensorFlow / Keras
* NumPy
* Pandas
* Scikit-learn
* Matplotlib
* Streamlit
* Jupyter Notebook

## Project Structure

```text
.
├── embedding.ipynb          # Notebook for understanding word embeddings
├── simplernn.ipynb          # Model training using Simple RNN
├── prediction.ipynb         # Prediction and model testing notebook
├── main.py                  # Streamlit web application
├── simple_rnn_imdb.h5       # Trained Simple RNN model
├── requirements.txt         # Required Python libraries
└── README.md                # Project documentation
```

## How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/Hritik827/Imdb-sentiment-analysis-simple-rnn.git
cd Imdb-sentiment-analysis-simple-rnn
```

### 2. Create a Virtual Environment

```bash
python -m venv venv
```

Activate the environment:

For Windows:

```bash
venv\Scripts\activate
```

For Mac/Linux:

```bash
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the Streamlit App

```bash
streamlit run main.py
```

After running the command, open the local Streamlit URL shown in the terminal.

## Example Usage

Enter a movie review such as:

```text
The movie was amazing. The story was emotional and the acting was excellent.
```

The app will return:

```text
Sentiment: Positive
```

Another example:

```text
The movie was boring and the plot was very weak.
```

The app will return:

```text
Sentiment: Negative
```

## Model Details

The model uses a Simple Recurrent Neural Network to process sequential text data. The IMDB dataset is converted into integer sequences, padded to a fixed length, and passed through the neural network for binary classification.

The output score is interpreted as:

* Score greater than 0.5: Positive sentiment
* Score less than or equal to 0.5: Negative sentiment

## Learning Outcome

Through this project, I practiced:

* Natural Language Processing preprocessing
* Word indexing and sequence padding
* Building a Simple RNN using TensorFlow/Keras
* Saving and loading trained deep learning models
* Creating an interactive ML app using Streamlit
* Deployable project structure for GitHub portfolio

## Future Improvements

* Add LSTM and GRU models for comparison
* Improve text preprocessing
* Add model performance metrics and visualizations
* Deploy the Streamlit app online
* Add a better UI with confidence score visualization

## Author

**Hritik Vivek Patil**

## License

This project is for educational and portfolio purposes.
