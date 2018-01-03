# Lie-Detector
This is a very simple one layer neural network to analyze lies through text messages.

Hey guys i am a just a teen who freshly started out with neural networks.Recently i read this research about human psychology where it said about the different techniques of catching lies through text messages.
The links to that are as follows:
  1>https://www.enkirelations.com/how-to-tell-if-someone-is-lying-over-text.html
  2>http://www.dailymail.co.uk/sciencetech/article-2821767/The-language-LYING-Expert-reveals-tiny-clues-way-people-talk-reveal-withholding-truth.html
  
I think there are some ted talks on it too.
 
I wrote the code in python and I have implemented a lot of it from Toby Segarans's "Programming Collective Intelligence"
  
The code is all finished, all that is left is to train the net. I trained it to some extent, but being a high school student its hard to spend a lot of time on extra-curricular projects.

I hope there are some people out there wiiling to help me train it properly. Any help is appreciated may it be improving the code or training it.And please bear with me if i made any mistakes because im new to both ML and github.
------------------------------------------------------------------------------------------------------------------------------------------
This code accepts a sentence and splits it into words using the split function in the searchnet class in module nn.py. It then stores it in a database ids.db. Them the actual working takes place in Truth.db.

To train the net use the function - train(self,word,ans) where word is the sentence(or the text) and the ans is if it is a true or false statement(0 means false and 1 means true).
eg:

>a = nn.searchnet("Truth.db")

>a.train("I did not do this",1)

To get the result of a particular sentence being true or false use the function - getresult(self,word) where for word is the sentence
eg:

>a = nn.searchnet("Truth.db")

>a.getresult("I did not do this")

[0.223,0.424]

The left value is the false value and the right value is the true value

PS:While training please input all words in lowercase except I

Any help would be greatly appreaciated :-)
