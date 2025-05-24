# Sentence Autocompletion with TensorFlow & Flask

This project demonstrates how to build a sentence autocompletion model using an LSTM neural network with TensorFlow, and deploy it as a web application using Flask.

# Features
Text Prediction: Generates autocomplete suggestions for partial sentences.

Deep Learning Model: Built using LSTM (Long Short-Term Memory) networks.

Web Interface: Simple Flask web app to interact with the model.

# Prerequisites
Python 3.x

TensorFlow 2.x

Flask

Other Python dependencies listed in requirements.txt

# Installation
# Step 1: Clone the repository
bash
Copy
Edit
git clone https://github.com/your-repository/sentence-autocompletion.git
cd sentence-autocompletion
# Step 2: Create a virtual environment
For better dependency management, it's recommended to create a virtual environment.

bash
Copy
Edit
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
# Step 3: Install dependencies
Install all the required Python packages:

bash
Copy
Edit
pip install -r requirements.txt

# Step 4: Prepare the Dataset
Download the dataset (e.g., a corpus of Shakespeare’s works or any text dataset).

Place the dataset (in CSV format) into the project folder.

The dataset should have a column named PlayerLine containing text data.

# Step 5: Train the Model
Run train_model.py to preprocess the text data and train the LSTM model.

bash
Copy
Edit
python train_model.py
This will:

Clean the text data.

Tokenize and vectorize the text.

# Train an LSTM model.

Save the model (sentence_completion.h5) and tokenizer (tokenizer.pkl) to disk.

# Step 6: Run the Flask App
After training the model, you can start the Flask app:

bash
Copy
Edit
python app.py
This will start a web server. You can access the app at http://localhost:5000.

# Step 7: Interact with the Web App
Go to the web interface at http://localhost:5000.

Enter a partial sentence and specify how many words you want to autocomplete.

Click "Generate" to see the predictions.


# License
This project is licensed under the MIT License - see the LICENSE file for details.
