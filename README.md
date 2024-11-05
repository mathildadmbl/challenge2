# challenge2

## Comments from the teacher : 

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

## FEATURES DESCRIPTION 

1. **FILENAME**: Identifier for the dataset entry; can be ignored.
2. **URL**: The URL of the website.
3. **URLLength**: Length of the URL.
4. **Domain**: Domain name in the URL.
5. **DomainLength**: Length of the domain name.
6. **IsDomainIP**: Indicates if the domain is an IP address (1) or not (0).
7. **TLD**: Top-level domain (e.g., .com, .org).
8. **URLSimilarityIndex**: Similarity measure with known legitimate URLs.
9. **CharContinuationRate**: Rate of continuous characters in the URL.
10. **TLDLegitimateProb**: Probability of the TLD being legitimate.
11. **URLTitleMatchScore**: Match score between URL and page title.
12. **URLCharProb**: Probability distribution of characters in the URL.
13. **DomainEntropy**: Entropy measure of the domain name.
14. **SubDomainCount**: Number of subdomains in the URL.
15. **DomainAge**: Age of the domain (in days).
16. **PageRank**: Page rank of the website.
17. **AlexaRank**: Alexa ranking of the website.
18. **HTTPS**: Indicates if the URL uses HTTPS (1 for yes, 0 for no).
19. **HasRedirect**: Indicates if there’s a redirect in the URL (1 for yes, 0 for no).
20. **URLDepth**: Depth of the URL (number of “/”).
21. **NumSpecialChars**: Number of special characters in the URL.
22. **NumDigits**: Number of numeric digits in the URL.
23. **NumKeywords**: Number of known phishing keywords in the URL.
24. **IsSuspiciousExtension**: Indicates if the URL has a suspicious file extension (1 for yes, 0 for no).
25. **PhishingLabel**: Label indicating if the URL is legitimate (1) or phishing (0). 

