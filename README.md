# Chimi-Bot Service
A slack bot that will allow members to award chimichangas to each other and will track totals for bragging rights.

## This will be:
- A service that will listen for messages from the Slack API, then update a dataabase accordingly.
- Have bi-monthly totals posted to the Chimi-Bot Home channel.
- Use a lightweight data structure to ensure efficiency and stability.
- Only save the info relevant to the app:
    - How many chimi's were given?
    - Who gave the chimi?
    - Who received the chimi?

## How to use it:
Once the application has been added to your Slack organization, use is as simple as opening a team channel, then writing a message that contains a person's Slack username and a :burrito: emoji.  A maximum of 7 chimichangas can be given each day.
- Example: "Hey @mike, thank's for your help with those reports! :burrito: :burrito:"
- Example: "@melissa, :burrito: time!"

The app will track who got how many chimichanga's, from whom, and what date.  Otherwise, no potentially sensative information will be saved.  Twice a month, Chimi-Bot will post an updated leaderboard (both sends and receives) to the Chimi-Bot home channel.

## Tech involved?
My initial thought is to use python (I'm teaching it to myself now) and then use AWS Lambda to run the processes rather than have a constantly running application that may not get used frequently.  Database could be lightweight, and should only need one or two tables.

