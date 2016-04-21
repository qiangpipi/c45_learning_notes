# c45_learning_notes #

This is a learning notes of C4.5 which described in the book "The Top Ten Algorithms in Data Mining"  

### Learning Data Set ###

|Day|Outlook|Temperature|Humidity|Windy|Play Golf?|
|---|---|---|---|---|---|
|1|Sunny|85|85|False|No|
|2|Sunny|80|90|True|No|
|3|Overcast|83|78|False|Yes|
|4|Rainy|70|96|False|Yes|
|5|Rainy|68|80|False|Yes|
|6|Rainy|65|70|True|No|
|7|Overcast|64|65|True|Yes|
|8|Sunny|72|95|False|No|
|9|Sunny|69|70|False|Yes|
|10|Rainy|75|80|False|Yes|
|11|Sunny|75|70|True|Yes|
|12|Overcast|72|90|True|Yes|
|13|Overcast|81|75|False|Yes|
|14|Rainy|71|80|True|No|

From the data set table:  
- The possibility to "Play Golf" is 9.0/14.0;  
- The possibility not to "Play Golf" is 5.0/14.0;  
- The entropy of the "Play Golf?"  
<img src="http://www.forkosh.com/mathtex.cgi?sum_{i=0}^n-p_{i}log_2%20p_{i}">  
    = -(9.0/14.0)*log2(9.0/14.0)-(5.0/14.0)log2(5.0/14.0)  
    = 0.945934  

### Test for column "Day" ###
### Test for column "Outlook" ###
Gain(Outlook) = Entropy(PlayGolf? in Outlook) - Sum
### Test for column "Windy" ###
