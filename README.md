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
