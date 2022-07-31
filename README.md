# chatbot-using-python
this is friendly chatbot project give 

# chatbot-using-python
this is friendly chatbot project give people nice answers about their questions, build with many tools and modules like (random module, word_tokenize, lemmatizer, bag of words, Sequential, SGD,..)

 -using ( random ) module to get random responses 
- read and load the ( data_file ), then loop through  the (intents , patterns)
 
         Processing Data 
- use ( word_tokenize ) to separate words
- use ( words.extend ) to move words into ( words ) empty List then append words from words empty list to the appropriate intent tag.
- using (lemmatizer) to decrease words and remove duplicates words, then sort classes.
- save the processed words to (words.pkl ) file to save the time of reprocessing words again.
- convert words to vectors and  create training list then create empty array for the outputs.
- Apply ( bag of words ) by converting words to numerical values (1, 0), So the output will be ( 1 ) for the current available tag and ( 0 ) for other tags.
- shuffle the features in training data and convert it to an np array using (.shuffle), then create train and test lists 

        Create the model 
Create model with ( Sequential ) model from Keras with parameters like (Dense, Dropout ) 

          Complie the model 
- compile the model with ( Stochastic gradient descent ) because we have multiple outputs.
        - Fitting and saving the model 
Finally we fit the model and save it.


- create another python file and load the model inside it, then tokenize and lemmatize words
- return words to bag of words array ( " 1 " if the word exist and " 0 " if the word not exist )
- predict class based on tags ( "greeting " or " thanks " or anything else ) then sort it by the strength of probality.

- pick a random response from (intents.json) file then get a chatbot response.

- creating GUI with (tkinter) which return the results from (( return res )) 
 - finally create chat window and all of it's properties and customization.
