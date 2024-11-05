# challenge2

Comments from the teacher : 

Goal: classify websites depending on whether they are phishing websites or not 
- each row is a website 
- each column is an attribute
- last column: flag 0 (phising) 1 (legitimate) 
  
Some of the attributes are raw : url, domain name 
Some are statistics computed from the url or the html content of the website : based on the kind of characters, what is inside the html (the content, suspicious code, javascript to get data in a hidden way …)

We have to remove the high level attributes that are computed not only from the websites but by comparing them to a large list of legitimate websites 
bc one technique for phishing is to produce an url very similar to the legitimate one 
by comparing to the legitimate urls, we can have an idea 
a bit too much of an idea --> they might boost the score too much and have too much importance 
