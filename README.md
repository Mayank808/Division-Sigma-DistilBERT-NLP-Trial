# Division-Sigma-DistilBERT-NLP-Trial
We tried our best to use a DistilBert model in order to do sentiment analysis on a data set!!
Performing data cleaning and preprocessing:

We started the competition by trying to use the BERT model to make our predictions.  Bert does not accept un-clean input, so we have to parse and clean the sentences Bert receives beforehand. This means removing punctuation, tokenizing, masking and padding the sentences.  This is done using hugging tree's transformer library and the transformer tokenizer's batch_encode_plus(method).  This allows us to use preprocessing methods designed for BERT, and TensorFlow hub's KerasLayer implementation.

Before encoding the sentences the dataframe is split up into a training and validation set.

We tried to come up with our own methods for tokenization, however we ended up getting some help from https://www.tensorflow.org/official_models/fine_tuning_bert and made tweaks accordingly. 

Training the Model:

Using the TFBertModel resulted in extremely slow training with training times exceeding 300 hours.  Thus we switched to Distillbert. Which gave a 3+ hour training time, which for the distilbert model is way too high. We tried our best to fix it and also have time for training however we weren't able to find the issue in time and just started training the model. The training was going fine until the first epoch was about to finish where the training crashed. We had implemented checkpoints in order to avoid this however they didn't end up working lol. 

As a whole we tried our best to be ambitious and inquisitive by tring a model we had only a bit of experience with. Even though we weren't able to succeed we still learned a lot and tried our best. 


Ps. 
August 23rd as a day however was pretty the raptors managed to sweep the nets and it was also Kobes birthday so RIP the legend. Queue the COLDPLAY and pain playlist. 




