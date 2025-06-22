## TL;DR = Join Slack and get a personalized welcoming message

The flow code has 7 tasks:
1. Take true or false as input from the user to get an invite for the Slack workspace
2. If the user selects true, ask their name ( optional )
3. Get the user's IP Address using the ipify api
4. Use the IP Address to know the city the user is in and the ISP of the user using the ipinfo api
5. Provide the latest weather description along with temperature, humidity, and UV index as the Output using the weatherstack api
6. Query the data and provide the output in a paragraph with the needed information
7. Send the output as a welcoming message to the Slack workspace

- It utilises Switch cases for conditional logic
- It uses the Jsonata plugin to transform and query the JSON data received from the api request.
- It uses the Slack-notification plugin to send a message in the workspace after the task is successfully run.

 #### The purpose of the flow is to demonstrate the dynamic workflow orchestration capabilities of Kestra for an ETL (Extract, Transform, Load) pipeline use case.
 
You can join the Dummy Workspace to view the messages. Here is the invite [Link](https://join.slack.com/t/testingflow-group/shared_invite/zt-37wnj78jp-XFKCy7b0M3dgpAoTcg4kcQ#)

Resources:
1. https://www.ipify.org/
2. https://ipinfo.io/dashboard/ (Get your key)
3. https://weatherstack.com/dashboard (Get your key)
4. https://api.slack.com/ (Get your key)
5. https://kestra.io/docs 
6. https://docs.jsonata.org/overview.html

Disclaimer: The APIs used are under the free tier subscription, so if you run the flow  with VPN enabled or with Proxy, it will provide inaccurate data. 

#### The code has the necessary API Keys in the Docker Compose file for easy testing purposes. Users can replace them with their own. 
## How to test: 
Prerequisites: None!
### Steps
1. Copy [compose.yaml](https://github.com/thisiskaransgit/Kestra-FlowCode/blob/master/docker-compose.yml) and build the service
2. Start the Kestra Server
3. Copy [Kestraflow.yaml](https://github.com/thisiskaransgit/Kestra-FlowCode/blob/master/kestraflow.yaml)
4. Save the file and then execute.
5. The flow will ask for your response
6. If yes, then give your name as an input (optional)
7. Once the flow is done, head over to the output section to get the invite link for the workspace
8. In the workspace, you will receive a custom welcoming message.

## How to test with your credentials:
Prerequisites:
1. ipify api `no key`
2. IPInfo access key
3. Weatherstack access key
4. Slack workspace with required access
5. Slack incoming webhook access key
6. Docker compose [file](https://github.com/kestra-io/kestra/blob/develop/docker-compose.yml) downloaded
7. Kestra is installed and running
### Replace the given keys with your own and follow the above give steps


The project is made during  the [#KestraHackWeek](https://x.com/WeMakeDevs/status/1934454399360786763)
