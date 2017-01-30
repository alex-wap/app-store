# How-to Guide for Apple App Store Submittal


## Prerequisites
* [Apple Developer Account](https://developer.apple.com/)
* [Sign up for Apple Developer Program](https://developer.apple.com/account/#/membership/)
* Screenshots. You can generate these using the simulator and Command+S to take a screenshot. The bare minimum is one iPad Pro screenshot and one iPhone 7 Plus screenshot (highest resolutions for iPad and iPhone).
* 1024px X 1024px Image (your App Icon).
* Add App Icons to your project.
  * Go to Project - General - App Icons and Launch Images - App Icons Scource.
  ![app icons](https://github.com/alex-wap/app-store/blob/master/images/0.png "app icons")
  * Use Asset Catalog or create a new one.
  * Open assets folder in your project.
  * Use a Mac App [Prepo](https://itunes.apple.com/us/app/prepo/id476533227?mt=12) or make your own icons. 
  * **WARNING**, do not have duplicate icons (exact same size, but different name). **DOUBLE CHECK AND DELETE DUPLICATES**
  * Drag and drop your icons from the Finder into the assets folder in Xcode
* Have your project open in Xcode. 

## Instructions
* Log into Apple Developer Account
* Go to Certificates, Identifiers & Profiles
* Click Identifiers - App IDs - Create new App ID (plus button top right)
![new app id](https://github.com/alex-wap/app-store/blob/master/images/1.png "App IDs")
* App ID Description can be anything. Under "Explicit App ID", **you must match your "Bundle ID" in Xcode.**
* Continue. Submit.
* Click Provisioning Profiles - Distribution - Create new Provisioning Profile
![Provisioning Profile](https://github.com/alex-wap/app-store/blob/master/images/2.png "Provisioning Profile")
* Select *Distribution - App Store*. Continue.
* Select your App ID from the list. Continue.
* Select Certificate. Continue.
* Create Profile Name. Generate.
* Download Provisioning Profile and remember where it is.
* Go to [iTunes Connect](https://itunesconnect.apple.com/). 
* Go to My Apps.
* Click the plus button to create a "New iOS App".
* **Name field is permanent after submission. Pick what you want carefully.** 
* Create a name. Select English. Select your Bundle ID. Version 1.0. SKU is a unique ID (you pick it). e.g. TicTacToe0.1
* Name is required. Description is required. Keywords are required. 
* Support URL is required (your website or github). Private Policy URL is required (same link).
* Copyright (your business name) required.
* Address information is required.
* Category is required.
* Click edit next to "Rating". Fill out questionnaire. Be careful, **it's easier to get approved if you select "Not Made For Kids".**
* Fill out contact information for "App Review Information"
* You do not need a "Demo Account".
* Automatically release version.
* Click the Save button in the top right.
* Switch Tab to "Pricing".
* Select Price Tier "Free".
* Save.
* Switch to Xcode.
* Select your build target as "Generic iOS Device"
![build target](https://github.com/alex-wap/app-store/blob/master/images/3.png "build target")
* From the Top Menu Bar, Select **Product > Archive**
![archive](https://github.com/alex-wap/app-store/blob/master/images/4.png "archive")
* After Archiving, Find your Provisioning Profile file and double-click it from your Finder.
* Xcode will open the file.
* Click Validate. Loading Screen. Click Validate again.
* Wait for "Validation Successful". (long wait) Click Done.
  * Most errors will occur at this stage. Read the error messages and check Stack Overflow for solutions if they are not obvious.
* Click "Submit...". Select your Development Team. Click Choose.
* Click Submit. (long wait)
* Switch back to [iTunes Connect](https://itunesconnect.apple.com/).
* Click Save. Reload the iTunes Connect page.
* Your build may take several minutes to process before it will show up on the page.
* Go to Build (plus button). Add Build. Click Done.
* Save. Submit for Review. Follow instructions if you're missing information.
* Fill out information. "No" Export Compliance, "No" Content Rights, "No" Advertising Identifier.
* Click Submit.
* App is now "Waiting For Review". 
  * The next stages are:
  * "Preparing for Review"
  * "Going in Review"
  * "Accepted" or "Rejected" 
* You will receive an email for your app's approval, but it is good to check it yourself in [iTunes Connect](https://itunesconnect.apple.com/).

## Live Demo of Apple App Store Deployment


**Coming Soon**


## Alternative Video


[Jared Davidson - Submitting an App to the iOS App Store](https://www.youtube.com/watch?v=6uX7B8ZfMiw)