## TL;DR = Know the weather conditions of your city 

The flow code has 4 tasks:
 1. Get the user's IP Address 
 2. Use the IP Address to know the city you user is in 
 3. Provide the latest weather description along with temperature, humidity, and UV index as the Output
 4. Send the output as a message to the Slack workspace


This code utilises the Jsonata plugin to transform and query the JSON data received from the api request.
And it uses the Slack-notification plugin to send a message in the workspace after the successful run of the task.


The code has the necessary API Keys in the Docker Compose file for easy testing purposes. Users are free to use their credentials for testing

#KestraHackWeek
