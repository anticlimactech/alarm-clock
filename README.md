# Scott Watkins
CS4320 Alarm Clock Use Case and Description

*The clock shows the time of day. Using buttons, the user can set the hours and minutes fields individually, and choose between 12 and 24-hour display.*

*It is possible to set one or two alarms. When an alarm fires, it will sound some noise. The user can turn it off, or choose to “snooze”. If the user does not respond at all, the alarm will turn off itself after 2 minutes. “Snoozing” means to turn off the sound, but the alarm will fire again after some minutes of delay. This “snoozing time” is pre-adjustable.*

![Use Case Diagram](AlarmClockUseCaseDiagram.png)

**Use Case Description**
- User is able to Set Current Time, which will include cases for to Set 12 or 24 Hour Format, Set Hours, and Set Minutes.
- User can Set Alarm Time for up to two separate alarms, which includes Set Hours and Set Minutes.
- User can Set Snooze Duration, which includes Set Minutes.
- If user has Set Alarm Time, Play Sound When Alarm Fires extends Set Alarm Time cases. User will be able to Snooze or Turn Off the Alarm.
- If Play Sound When Alarm Fires case is not turned off or snoozed after 2 minutes, Snooze is included and Alarm will Fire again after Snooze Duration has passed.