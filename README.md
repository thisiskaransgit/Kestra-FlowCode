## TL;DR = Know the weather conditions of your city 

The flow code has 4 tasks:
 1. Get the user's IP Address using ipify api
 2. Use the IP Address to know the city the user is in using ipstack api
 3. Provide the latest weather description along with temperature, humidity, and UV index as the Output using the weatherstack api
 4. Query the data and provide the output in a paragraph with the needed information
 5. Send the output as a message to the Slack workspace

- This code utilises the Jsonata plugin to transform and query the JSON data received from the api request.
- It uses the Slack-notification plugin to send a message in the workspace after the task is successfully run.


The code has the necessary API Keys in the Docker Compose file for easy testing purposes. Users are free to use their credentials for testing 


#KestraHackWeek
