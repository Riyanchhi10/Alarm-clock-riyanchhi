# Alarm-clock
Simple alarm clock website using HTML, CSS and JS .
PF https://riyanchhi10.github.io/Alarm-clock-riyanchhi/ .

script.js -
This JavaScript code defines an alarm clock application. Let's break down the code step by step:

The code starts by declaring variables and selecting elements from the HTML document using document.getElementById() method. These elements include:

time: An element to display the current time.
dateInput: An input element for selecting the alarm date.
tInput: An input element for selecting the alarm time.
btn: A button element to set the alarm.
contan: A container element to hold the list of alarms.
interVal: A variable to hold the reference to the setTimeout or setInterval function.
maxValue: Maximum number of alarms allowed (set to 3).
cnt: Counter to keep track of the number of alarms set.
almTimesArray: An array to store the selected dates for alarms.
timeChangeFunction() is a function that updates the displayed time every second. It retrieves the current time using new Date() and formats it to HH:MM:SS AM/PM format.

alarmSetFunction() is called when the user clicks the "Set Alarm" button. It checks if the selected alarm time is in the future and if it's not a duplicate alarm. If conditions are met, it calculates the time until the alarm and creates a new alarm element to display. The alarm element contains the selected date and a delete button. It also sets a timeout to trigger an alert when the alarm time is reached.

showAlarmFunction() is a helper function to handle the deletion of alarms. It iterates over all existing alarm elements and adds event listeners to their delete buttons to remove them.

showAlarmFunction() is called initially to set up the event listeners for alarm deletion.

timeChangeFunction() is called initially to display the current time.

Finally, setInterval(timeChangeFunction, 1000) is set up to update the displayed time every second.

Overall, this code creates an alarm clock interface allowing users to set up to three alarms and receive alerts when the alarm time is reached.

