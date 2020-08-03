# Simple RASA Chatbot App
This is simple application of chatbot built using RASA framework that saves information in Slots and check for email validation by regex (regular expression) using Python programming language.

## Getting Started
Clone the project and use the flag "pipenv shell" that will spawn a shell with the virtualenv activated and will solve the dependencies requirements.

### Prerequisites
1. Install the Python development environment
2. Install pipenv for building virtual environment (strongly recommended)
3. Install Rasa Open Source (if not using pipenv)

For more information about the prerequisites you can check out this documentation https://rasa.com/docs/rasa/user-guide/installation/#installation-guide

### Train the Model
To train the model you can run the "rasa train" command on your command line.
This command trains the model using NLU data and stories and save the model in ./models directory.

### Running the Project
After training the model, you can try out the project by running "rasa shell" command on your command line.
You can talk to the assistant and see for the bot reaction.

### Evaluating the Model
To evaluate the model you can run the "rasa test" command on your command line.
This will output performance evaluation metrics according to the test stories.
