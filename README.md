This agent will generate a daily literature digest for Dai lab members by searching Pubmed using the provided keywords.
The digest is scheduled to be sent at 7:00 AM each day for papers published in the previous day.

In summary, the daily-digest-agent script:
1. Searches PubMed for articles from yesterday that match some PAH-related keywords.
2. Constructs a neatly formatted HTML table of those articles.
3. Emails that table as a “Daily Dai Lab Literature Digest” to a list of recipients.

This YAML file serves the following purpose:
GitHub reads it and sets up an automation pipeline (“workflow”) that:
1. Runs every day at a specific UTC time.
2. Installs Python and its dependencies.
3. Executes the daily_digest_agent.py script with the appropriate environment variables retrieved from GitHub Secrets.
