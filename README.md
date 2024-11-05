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

1. **FILENAME**: An identifier for the dataset entry; this column can be ignored.
2. **URL**: The actual URL of the website.
3. **URLLength**: The length of the URL.
4. **Domain**: The domain name extracted from the URL.
5. **DomainLength**: The length of the domain name.
6. **IsDomainIP**: Indicates whether the domain is an IP address (1) or not (0).
7. **TLD**: The top-level domain of the URL (e.g., .com, .org).
8. **URLSimilarityIndex**: A measure of similarity between the URL and known legitimate URLs.
9. **CharContinuationRate**: The rate at which characters continue without interruption in the URL.
10. **TLDLegitimateProb**: The probability that the top-level domain is associated with legitimate websites.
11. **URLTitleMatchScore**: A score indicating the match between the URL and the webpage title.
12. **URLCharProb**: The probability distribution of characters in the URL.
13. **DomainEntropy**: The entropy measure of the domain name, indicating randomness.
14. **SubDomainCount**: The number of subdomains in the URL.
15. **DomainAge**: The age of the domain in days.
16. **PageRank**: The PageRank score of the website.
17. **AlexaRank**: The Alexa ranking of the website.
18. **HTTPS**: Indicates whether the URL uses HTTPS (1) or not (0).
19. **HasRedirect**: Indicates the presence of redirection in the URL (1 for yes, 0 for no).
20. **URLDepth**: The depth of the URL, determined by the number of '/' in the path.
21. **NumSpecialChars**: The number of special characters in the URL.
22. **NumDigits**: The number of numeric digits in the URL.
23. **NumKeywords**: The number of known phishing-related keywords in the URL.
24. **IsSuspiciousExtension**: Indicates if the URL has a suspicious file extension (1 for yes, 0 for no).
25. **PhishingLabel**: The label indicating if the URL is legitimate (1) or phishing (0).
26. **NumDots**: The number of dots ('.') in the URL.
27. **NumHyphens**: The number of hyphens ('-') in the URL.
28. **NumUnderscores**: The number of underscores ('_') in the URL.
29. **NumEqualSigns**: The number of equal signs ('=') in the URL.
30. **NumAmpersands**: The number of ampersands ('&') in the URL.
31. **NumExclamations**: The number of exclamation marks ('!') in the URL.
32. **NumAsterisks**: The number of asterisks ('*') in the URL.
33. **NumPercentSigns**: The number of percent signs ('%') in the URL.
34. **NumTildes**: The number of tildes ('~') in the URL.
35. **NumCommas**: The number of commas (',') in the URL.
36. **NumPlusSigns**: The number of plus signs ('+') in the URL.
37. **NumPipes**: The number of pipe symbols ('|') in the URL.
38. **NumSlashes**: The number of forward slashes ('/') in the URL.
39. **NumBackslashes**: The number of backslashes ('\\') in the URL.
40. **NumColons**: The number of colons (':') in the URL.
41. **NumSemicolons**: The number of semicolons (';') in the URL.
42. **NumQuestionMarks**: The number of question marks ('?') in the URL.
43. **NumAtSymbols**: The number of at symbols ('@') in the URL.
44. **NumHashes**: The number of hash symbols ('#') in the URL.
45. **NumSpaces**: The number of spaces (' ') in the URL.
46. **NumTLDs**: The number of top-level domains in the URL.
47. **NumParams**: The number of parameters in the URL.
48. **NumFragments**: The number of fragments in the URL.
49. **NumSubdomains**: The number of subdomains in the URL.
50. **IsShortenedURL**: Indicates if the URL is shortened (1 for yes, 0 for no).
51. **HasMailTo**: Indicates the presence of 'mailto:' in the URL (1 for yes, 0 for no).
52. **HasJavaScript**: Indicates the presence of 'javascript:' in the URL (1 for yes, 0 for no).
53. **HasData**: Indicates the presence of 'data:' in the URL (1 for yes, 0 for no).
54. **HasVBScript**: Indicates the presence of 'vbscript:' in the URL (1 for yes, 0 for no).
55. **HasAbout**: Indicates the presence of 'about:' in the URL (1 for yes, 0 for no).
56. **HasFile**: Indicates the presence of 'file:' in the URL (1 for yes, 0 for no).

