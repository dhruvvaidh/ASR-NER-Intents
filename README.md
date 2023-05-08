# Automatic Speech Recognition, Entity and Intent classification and Text Summarization

## Automatic Speech Recognition(ASR) using SpeechRecognition (Task-1)
API Used: Google API(recognize_google())
Libraries used:
1. pydub
2. SpeechRecognition

### Steps involved in ASR:
1. Import the audio file
2. Split the audio into segments using split_on_silence() from the pydub library
3. Import the SpeechRecognition library and initialise the Recognizer class
4. Use recognize_google() on each and every segment created before and append them into a list
5. Combine the sentences to form a paragraph

## Intent and Entity extraction(Task-2):
Libraries used: transformers, spacy, pytorch

### Steps involved in Entity and Intent Classification

*Steps involved in Intent Classification:*
1. Creating a Dataset of custom intents and examples
2. Downloading the model and it's tokenizer
3. Tokenizing the input texts and making a pytorch dataset for the model
4. Training the model
5. Performing Intent Classification on each and every sentence extracted before
6. Storing the output in a dictionary

*Steps involved in Entity Classification:*
1. Import the spacy library and the en_core_web_sm model
2. Load the model in the nlp object
3. Create a document for each and every sentence extracted before
4. Perform NER on each and every sentence extracted before
5. Storing the output in a dictionary

Then we combine the outputs of all the steps mentioned above into a one dictionary.

## Storing the outputs in a JSON file(Task-3):
Libraries used: json

1. import the json library
2. Then use json.dump() to store the list of dictionaries achieved in the previous task

## Text-Summarization(Task-4)
Libraries used: sumy

1. Import the PlaintextParser,Luhn Summarizer, Tokenizer and stopwords
2. Initialize the summarizer with LuhnSummarizer
3. Set summarizer parameters
4. Initialize parser and tokenize
5. Generate summary
6. Print the summary




