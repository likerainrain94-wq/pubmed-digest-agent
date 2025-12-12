This agent will generate a daily literature digest for Dai lab members by searching Pubmed using the provided keywords.
The digest is scheduled to be sent at 7:00 AM each day for papers published in the previous day. 

In short, the script:
	1.	Searches PubMed for articles from yesterday that match some PAH-related keywords.
	2.	Builds a nicely formatted HTML table of those articles.
	3.	Emails that table as a “Daily Dai Lab Literature Digest” to a list of recipients.
