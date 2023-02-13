# German-To-English-Translator
Step 1

First, I have imported all the libraries
![image](https://user-images.githubusercontent.com/98225415/218530807-b36ee522-a653-40db-b5e8-17c72e1ab6f4.png)

Step 2

For the data, I have used the dataset provided by ManyThings.org website. The website has a lot of great datasets for phrases and translations in various languages. I have download the data set from the link provided here: https://raw.githubusercontent.com/jbrownlee/Datasets/master/deu.txt

Step 3

Now I have load the data and clean the data like removed non-printable characters and symbols ,removed all the punctuations in the data,normalized to ASCII
,maked all the characters lowercase,removed all the non-alphabetic characters .

![image](https://user-images.githubusercontent.com/98225415/218532669-480712cb-c638-4536-bbeb-87984386b21c.png)

Step 4

After saving the pickles for the English-German phrases with cleaning and saving in the list, I have used the following function to load it into the code for training.

![image](https://user-images.githubusercontent.com/98225415/218533093-cdcf50bc-7ec4-425d-bb62-d01fa9bef189.png)

Then I have split the dataset into train and test list into three pickles to reduce the dataset to my use case.

![image](https://user-images.githubusercontent.com/98225415/218534819-f1dce043-3f9f-4b31-b817-a34f282bfc01.png)

Step 5

To train an LSTM with text, I took a tokenizer.I have used the following function to create a tokenizer:

![image](https://user-images.githubusercontent.com/98225415/218535179-b1fc35e6-85ba-4007-a8ef-77df25ee84fe.png)

Step 6
Then I have use one hot encoding for categorical data to convert into a form that can be used for ML algorithms to increase the accuracy of the model.

![image](https://user-images.githubusercontent.com/98225415/218552747-825a745c-1daa-4028-8431-d7313cc8609f.png)

Step 7 

Here I have use LSTM model and train the data prepare english and german tokenizer prepare training and validation data and defined it in the model.

![image](https://user-images.githubusercontent.com/98225415/218554060-de520105-ebe9-4a69-b5c0-7ca94f7d5356.png)

![image](https://user-images.githubusercontent.com/98225415/218554206-19051c47-36bd-4c1c-b82f-06b33f193238.png)

Step 8

Now the last work I had done was to test the model and check the accuracy of the model.

![image](https://user-images.githubusercontent.com/98225415/218554576-9cc96611-fc3a-485f-85df-84b6c3ce09aa.png)

![image](https://user-images.githubusercontent.com/98225415/218554694-494cbb4a-91be-4bfc-8e47-40bb327ab2bb.png)



