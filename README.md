# Notification-System
Display notifications to the player's screen in seconds!

# How to implement:
1) Download and import NotificationSystem.unitypackage in your Unity project.
2) Create an empty GameObject under the Canvas and attach the NotificationSystem.cs script to it.
3) Add the graphics and the text under it (The GameObject that contains the NotificationSystem.cs script should only have 1 child).
4) Attach the text to the "Notification Text" field in the Notification System script component in the Inspector.
5) Done!

# How to use:
- Reference the NotificationSystem.cs script from your desired manager script.
- Now you are ready to start showing notifications:
```CSharp
// The first parameter is the text of the notification and the second one is the time before it disappears.
notificationSystem.ShowNotification(new Notification("I am a notification!", 2f));
```
- You can show 2 or more consecutive notifications:
```CSharp
// The first parameter is the text of the notification and the second one is the time before it disappears.
notificationSystem.ShowNotification(new Notification("First one", 2f));
notificationSystem.ShowNotification(new Notification("Second one", 1f)); // Will show 2 seconds after the first starts.
```

# Notes:
- There should only be 1 child of the GameObject that contains the NotificationSystem.cs script.
