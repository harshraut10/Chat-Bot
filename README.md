# Chat-Bot
Developed a chatbot using a predefined intents dataset in JSON format with tags (classes like greetings, names), patterns, and responses (possible replies). Preprocessing involves nltk for tokenization and lemmatization. Built with TensorFlow, the model predicts classes, and a random response from the corresponding tag is given to the user.

Developed a chatbot based on predefined dataset called intents
This intents dataset is a json object that has tags, patterns and responses
The tag is the class of the sentence describing what the sentence is such as greetings, names etc
The patterns are the corresponding sentences that occur for that tag such as hi->greeting
The response tag are a set of sentences that the chatbot may pick to give reply for that particular tag, it can be randomised
The preprocessing steps involves making use of the nltk libraries such as word_tokenize and WordNetLemmatizer for preprocessing pf the dataset
Other libraries such as pickle and numpy are used
The model is built using a tensorflw model
The tags are generally used as classes and the patterns as the data for that class
The model is trained and saved
Now for prediction the input is taken from the user
Again text preprocessing is done by using the nltk library
First we use word_tokenize to break the sentences into words and then we use wordnetlemmatizer to bring the word to its base or root form
Then it is fed to the model for prediction
The model for a particular threshold decides which class is more suitable for that sentence 
The output of the model is a class 
We use this class to iterate over the intent dataset and a random response is picked and given to the user
