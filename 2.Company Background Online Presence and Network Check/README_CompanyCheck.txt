Company_Check.ipynb contains a technical demo on how a company background, online presence and network is being checked and verified.

Main Function of this notebook is written and run as-
cred_check(company_name,n1,n2,n3)
taking a company name as input and giving 'Fail to Authenticate', 'Low', 'Mid', or 'High' as output for level of credibility of company.
	-'Fail to Authenticate' if url to company official site are not the same across sources or Company CEO cannot be verified with google search from site(s) aside from its source
	-'Low' if the aforementioned criteria are fulfilled
	-'Mid' if the aforementioned criteria are fulfilled, awards stated on professional networking site(s) can be verified with google search from site(s) aside from its source, and size of network of employees on professional networking site(s) is > n1
	-'High' if the aforementioned criteria are fulfilled, company reviews from company review site(s) have similarities processed and measured using NLP and Sørensen–Dice <n2, and job openings stated on professional networking site(s) and company review site(s) >n3 
n1,n2,n3 are set to default at 100, 0.5 and 20 respectively without explicit input.


To run the notebook successfully, please make sure that the following criteria are fulfilled.
1. packages in requirements.txt are installed
2. chromedriver is within the same directory as Company_Check.ipynb
3. cred.txt is within same directory as Company_Check.ipynb has 
	-* email, //account email for Professional Network Site and Company Review Site
	-* password, //account password for Professional Network Site and Company Review Site
	- google-api-key //from https://developers.google.com/custom-search/v1/overview, 
	- google-cse-id  //search engine id

*Code provided demonstrates a method of low overhead to access such information, do obtain agreement from these sites to run scraping activities labelled Function A and B in navigational header within the notebook.

