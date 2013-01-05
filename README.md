ouya-csharp
===========

C# bindings for the OUYA Development Kit

To get your Mono for Android game showing up in the OUYA Launcher, you will need to:
- set the project to use API Level 16
- add the Launcher image (732x412 pixels) in Resources/Drawable-xhdpi/ouya_icon.png
- add the following IntentFilter attribute to your Activity class

    [IntentFilter(new[] { Intent.ActionMain }
        , Categories = new[] { Intent.CategoryLauncher, "ouya.intent.category.GAME" })]

Deploy the game to the device.  Now it will show up in the OUYA Launcher.