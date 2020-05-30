# llSPS-INT-208-AI Powered News Search App using the Watson Discovery Service
# Summary
The internet is home to enormous amounts of data that is updated every day. Organizations can connect this constant stream of information to gain understanding, plan strategies, and find opportunities. Enriched news data can help any application make dynamic connections across current events faster. An AI powered news app is thus created that helps to access one’s own news of interest has been created by mining web application using JavaScript, Node.js, and the Watson Discovery service. The following exercises take place
•	The app is hosted on the IBM Cloud
•	Code is written in Node.js, with the server-side using the Express framework and  a Slack interface is used to query the data
•	The pre-built Watson Discovery News collection is used.
•	The Watson Discovery service is accessed through the Watson Discovery API


# Description
A news mining web application is built with the Watson Discovery service using the Watson Node.js SDK. The app demonstrates two use cases using Watson Discovery News:
•	Search: Query for the most relevant new articles about a specific topic or subject. Because the news collection is pre-enriched with natural language processing, it can query not just on keywords or categories but also on concepts, sentiment, and relations to get richer search responses.
•	Sentiment analysis- The query specifies whether the searched news in positive, negative or neutral. 
•	Trending topics in the news: Identify popular topics over the past 24 hours. Topics can be general, or specific to an industry or category.







# Flow
 
1.	The user interacts with the Watson Discovery News Server via the app UI.
2.	User input is processed and routed to the Watson Discovery News Server.
3.	The Watson Discovery News Server sends user requests to the Watson Discovery Service.
4.	The Watson Discovery Service queries the Watson News Collection.
5.	The Watson Discovery Service responds to Slack search requests.


# Included components
•	Watson Discovery: A cognitive search and content analytics engine for applications to identify patterns, trends, and actionable insights.
•	Github: A web development platform used or version control. It helps to simplify the process of collaborating different projects. It works on files changes in the projects can easily be merged with the master branch of the project.
Featured technologies
•	Node.js: An asynchronous event driven JavaScript runtime, designed to build scalable applications
•	React: Javascript library for building User Interfaces
•	Express: A popular and minimalistic web framework for creating API and Web server
•	Slack: Slack is a cloud-based set of team collaboration tools and services with chat bot integration
•	Botkit: Framework for creating and managing chat bots

# Deployment options

 



# Troubleshooting
If you find an error while deploying to IBM Cloud using the Deploy to Cloud Foundry option
1.	If the Lite version is used then the memory space must be reduced from 256mb to 128 mb
2.	If it continues then in the Stage History, click the Redeploy button.

# Setting up node-red environment
1.	Go to ibm cloud website
2.	Type Node-red in the catalog

 
3.	Set up the Node-Red  dashboard.

4.	Go to the Resource list of the IBM Cloud, Click on the node-red dashboard , the dashboard redirects to the node-flow where the necessary code is inserted

 


 






# Sample Output
The user interface of the node red application looks in general like the figure below:
 


# SLACK INTEGRATION WITH THE NEWS APP
The following steps are followed while integrating the slack environment.
1. Configure Slack
To integrate a new Slack Bot into your existing Slack team, navigate to https://<my.slack.com>/apps/manage/custom-integrations, where <my.slack.com> is the Slack workspace that needs to be customize.
1.	From the Cutsom Integrations page, select the Bots option.
 
2, To add a new bot, select the Add Configuration button.
 
3.	Enter a username for the bot and click Add bot integration.
 
4.	Once created, save the API Token that is generated.
 


2. Configure the application to use the Slack bot
If the app runs locally...
1.	Edit the .env file and enter the Slack Bot API Token saved in the previous step.
# Slack
SLACK_BOT_TOKEN=<slack_bot_token>
2.	Restart the application.
Search from Slack
The slack bot will respond to certain key words, below is a sample dialog. Remember to @ the bot each time, or start a private chat. Make sure to invite your bot into other channels using /invite @<my bot>.
user: @helpbot hi
helpbot: Hello.

user: @helpbot news please
helpbot: Hi there! What news are you interested in?

user: @helpbot toronto raptors
helpbot: You want me to search for news articles about `toronto raptors`?

user: @helpbot yes
helpbot: OK searching...
 

# Links
1.	https://cloud.ibm.com/login
2.	https://www.ibm.com/cloud/get-started
3.	https://developer.ibm.com/tutorials/how-to-create-a-node-red-starter-application/
4.	https://nodered.org/
5.	https://github.com/watson-developer-cloud/node-red-labs
6.	https://www.youtube.com/watch?v=W3iPbFTAAds&feature=youtu.be
7.	https://developer.ibm.com/articles/introduction-watson-discovery/
8.	https://cloud.ibm.com/docs/services/discovery?topic=discovery-getting-started
9.	https://www.youtube.com/watch?v=kwmqJRDbv98&feature=youtu.be


# Learn more
•	Artificial Intelligence Code Patterns: Enjoyed this Code Pattern? Check out our other AI Code Patterns.
•	AI and Data Code Pattern Playlist: Bookmark our playlist with all of our Code Pattern videos
•	With Watson: Want to take your Watson app to the next level? Looking to utilize Watson Brand assets? Join the With Watson program to leverage exclusive brand, marketing, and tech resources to amplify and accelerate your Watson embedded commercial solution.
License
This code pattern is licensed under the Apache License, Version 2. Separate third-party code objects invoked within this code pattern are licensed by their respective providers pursuant to their own separate licenses. Contributions are subject to the Developer Certificate of Origin, Version 1.1 and the Apache License, Version 2.
Apache License FAQ
