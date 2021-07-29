# Team Vacation Calendar App Script

This solution uses Google Apps Script to automatically populate a shared vacation calendar based on the individual calendars of each person on the team. When someone books time off they just need to remember to add an event to their personal Google Calendar using a keyword like "Vacation" or "Out of office." The script acts behind the scenes, scanning the calendars of all the members in a Google Group and syncing appropriate events to the shared calendar.

More information on how this script works can be found here: https://github.com/googleworkspace/solutions/tree/master/vacation-calendar

### Note : For the script to work you will need to:

1. Add the Google Calendar API (Under "Services" on the App Script editor).
2. Add the Admin SDK service (Under "Services" on the App Script editor).

### Common Errors

1. Error: Triggers are already set up - This occurs because a trigger is created automatically the first time the script is executed. If you need to run the script manually, first delete any existing triggers.
2. Failure to retrieve group members - Make sure the Admin SDK service has been added.
3. Failure to retrieve group member calendar events - This solution only accesses Calendar events that your colleagues have made visible to you via their privacy settings.
4. Failure to add calendar events to team calendar - Make sure the correct calendar ID has been added and that you have access to that calendar.

