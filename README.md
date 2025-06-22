## TL;DR = Join Slack and get a welcoming message

The flow code has 7 tasks:
1. Take true or false an input from user to get a invite for slack workspace
2. If the user selects true, ask their name ( optional )
3. Get the user's IP Address using ipify api
4. Use the IP Address to know the city the user is in and the isp of user using ipinfo api
5. Provide the latest weather description along with temperature, humidity, and UV index as the Output using the weatherstack api
6. Query the data and provide the output in a paragraph with the needed information
7. Send the output as a welcoming message to the Slack workspace

- It utilises Swith cases for conditional logic
- This code utilises the Jsonata plugin to transform and query the JSON data received from the api request.
- It uses the Slack-notification plugin to send a message in the workspace after the task is successfully run.
 
You can join the Dummy Workspace to view the messages. Here is the invite [Link](https://join.slack.com/t/testingflow-group/shared_invite/zt-37wnj78jp-XFKCy7b0M3dgpAoTcg4kcQ#)

The code has the necessary API Keys in the Docker Compose file for easy testing purposes. Users can replace them with their own. 
Resources:
1. https://www.ipify.org/
2. https://ipinfo.io/dashboard/ (Get your key)
3. https://weatherstack.com/dashboard (Get your key)
4. https://api.slack.com/ (Get your key)
5. https://kestra.io/docs 
6. https://docs.jsonata.org/overview.html

#KestraHackWeek
