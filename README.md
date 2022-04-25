# NLP-Business-Detection

## 1. Problem
Utilize several text data sources to automatically classify business operations.

## 2. Data
### Sources:
Employer internel data
### Data Dictionary:
SIC8 Description: description of standard industry code that the business belongs to

4_Square_Description: description of the business provided by one of our data providers

web_text: webtext based on the scrapped webtext of the given url

## 3. Model
Use BERT for embedding, followed by one decoder.

BERT + MLP

BERT + RNN

BERT + MLP (two texts)

BERT + CNN (two texts)

## 4. Results

Final optimal model: BERT + RNN

test accurcay: 84%

## 5. Improvements
Try the following given more time:

1. Try other embedding pretraining model, like GloVe, Word2Vec
2. Web_text doesn't improve much model accuracy, but instead increase the model training time. May need further look into this, like build a dictionary, or do some heavy cleaning
3. Didn't have enough time to tune hyperparameters, I believe the model performence will increase after tuning.

## 6. Reference
https://github.com/bentrevett/pytorch-sentiment-analysis

Refer to the use of torchtext in this tutorial, kudos to this brilliant work.

