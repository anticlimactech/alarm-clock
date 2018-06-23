# Scott Watkins
CS4320 Alarm Clock Use Case and Description

*The clock shows the time of day. Using buttons, the user can set the hours and minutes fields individually, and choose between 12 and 24-hour display.*

*It is possible to set one or two alarms. When an alarm fires, it will sound some noise. The user can turn it off, or choose to “snooze”. If the user does not respond at all, the alarm will turn off itself after 2 minutes. “Snoozing” means to turn off the sound, but the alarm will fire again after some minutes of delay. This “snoozing time” is pre-adjustable.*

![Use Case Diagram](AlarmClockUseCaseDiagram.png)

|  |  |
| --- | --- |
| **Name** | Set Current Time |
| **Description** | The current time will be displayed on the app. User is able to Set Current Time, which will include buttons for Set 12 or 24 Hour Format, Set Hours, and Set Minutes. |
| **Actors** | User |
| **Triggers** | User selects option to edit current time |
| **Pre-Condition** | Previously set time is displayed |
| **Post-Condition** | Time updated to user specification |
| **Main Course** | User clicks increment or decrement buttons to change hours and/or minutes until desired time is achieved |
| **Alternate Courses** | User clicks button to toggle between 12 and 24 hour time format |
| **Exceptions** | User selects button to cancel setting time |

&nbsp;

|  |  |
| --- | --- |
| **Name** | Set Alarm 1 Time |
| **Description** | Allows the user to set or change a time for alarm 1 to fire |
| **Actors** | User |
| **Triggers** | User selects button to set alarm time |
| **Pre-Condition** | Alarm not currently firing |
| **Post-Condition** | Alarm will sound once current time reaches set alarm time |
| **Main Course** | User clicks increment or decrement buttons to change hours and/or minutes until desired alarm time is achieved |
| **Alternate Courses** | User disables alarm |
| **Exceptions** | User selects button to cancel setting alarm |

&nbsp;

|  |  |
| --- | --- |
| **Name** | Set Alarm 2 Time |
| **Description** | Allows the user to set or change a time for alarm 2 to fire |
| **Actors** | User |
| **Triggers** | User selects button to set alarm time |
| **Pre-Condition** | Alarm not currently firing |
| **Post-Condition** | Alarm will sound once current time reaches set alarm time |
| **Main Course** | User clicks increment or decrement buttons to change hours and/or minutes until desired alarm time is achieved |
| **Alternate Courses** | User disables alarm |
| **Exceptions** | User selects button to cancel setting alarm |

&nbsp;

|  |  |
| --- | --- |
| **Name** | Set Snooze Duration |
| **Description** | User can determine how long system waits to re-fire alarm after snooze button is pressed during a firing alarm |
| **Actors** | User |
| **Triggers** | Set Snooze Duration button selected |
| **Pre-Condition** | Alarm not currently firing and/or Snooze not disabled |
| **Post-Condition** | Quiet time between firing alarm and next firing alarm will be set to user-desired setting |
| **Main Course** | User clicks increment or decrement buttons to change minutes until desired snooze time is achieved, between 1 and 59 minutes|
| **Alternate Courses** | User selects button to disable Snooze function |
| **Exceptions** | User selects button to cancel Snooze Duration edit |

&nbsp;

|  |  |
| --- | --- |
| **Name** | Snooze |
| **Description** | User may press a button to silence alarm for Snooze Duration previously set |
| **Actors** | User; System |
| **Triggers** | User presses Snooze button during firing alarm; No input for 2 minutes during firing alarm |
| **Pre-Condition** | Alarm currently firing; Snooze duration set |
| **Post-Condition** | Alarm discontinues firing for previously set Snooze Duration |
| **Main Course** | User selects button to Snooze alarm during an alarm firing. Alarm will silence for snooze duration |
| **Alternate Courses** | User may select button to disable alarm instead of snooze; system triggers snooze due to 2 minutes of inactivity during alarm firing |
| **Exceptions** | Snooze function is disabled, so user will not see Snooze option during alarm |

&nbsp;

|  |  |
| --- | --- |
| **Name** | Turn Off Alarm |
| **Description** | User turns off a firing alarm |
| **Actors** | User |
| **Triggers** | User selects button to turn off alarm during a firing alarm |
| **Pre-Condition** | Alarm time set; Alarm Firing |
| **Post-Condition** | Alarm silences |
| **Main Course** | During a firing alarm, user selects button to turn off alarm |
| **Alternate Courses** | User Snoozes alarm |
| **Exceptions** | N/A |