
SophiaH(ABND) [8:08 PM]
Hello @CharlesRowland.ProjectCoach, I have a question, here's my github: https://github.com/sharvey7/SophieInventoryAppPartOne I'm running my app and I don't see any errors yet for my project but it is showing error with my old project the news app: 10-10 03:21:46.489 5122-5122/? E/AndroidRuntime: FATAL EXCEPTION: main
   Process: harvey.ggc.edu.harveynewssecondpart, PID: 5122
   java.lang.RuntimeException: Unable to start activity ComponentInfo{harvey.ggc.edu.harveynewssecondpart/harvey.ggc.edu.harveynewssecondpart.SettingsActivity}: android.view.InflateException: Binary XML file line #2: Binary XML file line #2: Error inflating class fragment
       at android.app.ActivityThread.performLaunchActivity(ActivityThread.java:2646)
       
CharlesRowland.ProjectCoach [Oct 29th at 8:25 PM]
give me a few minutes ^_^


23 replies
SophiaH(ABND) [6 days ago]
Okay no problem


CharlesRowland.ProjectCoach [6 days ago]
have you cleared your logcat?


SophiaH(ABND) [6 days ago]
yes

CharlesRowland.ProjectCoach [6 days ago]
your app wont build for me

CharlesRowland.ProjectCoach [6 days ago]
it has build errors

CharlesRowland.ProjectCoach [6 days ago]
Screen Shot 2018-10-29 at 9.38.28 PM.png


SophiaH(ABND) [6 days ago]
Oh okay, I don't even see those errors yet

CharlesRowland.ProjectCoach [6 days ago]
do build > rebuild and then check the build menu on the bottom

SophiaH(ABND) [6 days ago]
Okay I'm waiting on it to build

SophiaH(ABND) [6 days ago]
Alright it says completed successfully in the build menu

SophiaH(ABND) [6 days ago]
Now I'll run my emulator again

SophiaH(ABND) [6 days ago]
Okay it's telling me about my project again. This error is showing:   --------- beginning of crash
10-30 03:42:25.650 8379-8379/? E/AndroidRuntime: FATAL EXCEPTION: main
   Process: harvey.ggc.edu.sophieinventoryapppartone, PID: 8379
   java.lang.RuntimeException: Unable to start activity ComponentInfo{harvey.ggc.edu.sophieinventoryapppartone/harvey.ggc.edu.sophieinventoryapppartone.MainActivity}: android.database.sqlite.SQLiteException: no such column: name (code 1): , while compiling: SELECT _id, name, price, quantity, supplier, phone FROM inventory
       at android.app.ActivityThread.performLaunchActivity(ActivityThread.java:2646)
       at android.app.ActivityThread.handleLaunchActivity(ActivityThread.java:2707)
       at android.app.ActivityThread.-wrap12(ActivityThread.java)

SophiaH(ABND) [6 days ago]
Is it saying something is wrong with my table?

CharlesRowland.ProjectCoach [6 days ago]
https://github.com/sharvey7/SophieInventoryAppPartOne/blob/master/app/src/main/java/harvey/ggc/edu/sophieinventoryapppartone/data/InventoryDbHelper.java
GitHub
sharvey7/SophieInventoryAppPartOne
Contribute to sharvey7/SophieInventoryAppPartOne development by creating an account on GitHub.
 

CharlesRowland.ProjectCoach [6 days ago]
```+ InventoryEntry.COLUMN_INVENTORY_PRICE + "INTEGER, "```

CharlesRowland.ProjectCoach [6 days ago]
you need a SPACE inbetween the " and INTEGER on all of the lines. so " SPACE type

CharlesRowland.ProjectCoach [6 days ago]
```+ InventoryEntry.COLUMN_INVENTORY_PRICE + " INTEGER, "```


CharlesRowland.ProjectCoach [6 days ago]
like that


SophiaH(ABND) [6 days ago]
oh so all of them need a space between the " and the datatype


CharlesRowland.ProjectCoach [6 days ago]
yup


CharlesRowland.ProjectCoach [6 days ago]
after you do that, uninstall the application and then rerrun it


SophiaH(ABND) [6 days ago]
okay I'll do that


SophiaH(ABND) [6 days ago]
Thanks so much!
