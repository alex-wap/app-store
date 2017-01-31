# How-to Guide for Apple App Store Submittal


## Prerequisites
* [Apple Developer Account](https://developer.apple.com/)
* [Sign up for Apple Developer Program](https://developer.apple.com/account/#/membership/)
* **Screenshots**. You can generate these using the Simulator and Command+S to take a screenshot. 
  * **REQUIRED** one iPad Pro screenshot.
  * **REQUIRED** one iPhone 7 Plus screenshot. 
  * These are the highest resolutions for iPad and iPhone.
* **1024px X 1024px Image** (your App Icon).
* Add App Icons to your project.
  * Go to Project - General - App Icons and Launch Images - App Icons Scource.
  ![app icons](https://github.com/alex-wap/app-store/blob/master/images/0.png "app icons")
  * Use Asset Catalog or create a new one.
  * Open assets folder in your project.
  * Use a Mac App [Prepo](https://itunes.apple.com/us/app/prepo/id476533227?mt=12) or make your own icons. 
  * **WARNING**, do not have duplicate icons (exact same size, but different name). **DOUBLE CHECK ACTUAL SIZE OF ICONS AND DELETE DUPLICATES**
  * Bare minimum 19 sizes for App Icons (in pixels):
    * 20x20
    * 29x29
    * 40x40 
    * 57x57
    * 50x50
    * 58x58
    * 60x60 
    * 72x72
    * 76x76
    * 80x80
    * 83.5x83.5
    * 87x87
    * 100x100
    * 114x114
    * 120x120
    * 144x144
    * 152x152
    * 167x167
    * 180x180
  * Drag and drop your icons from the Finder into the assets folder in Xcode
* Have your project open in Xcode. 

## Instructions
* Log into Apple Developer Account
* Go to Certificates, Identifiers & Profiles
* Click Identifiers - App IDs - Create new App ID (plus button top right)
![new app id](https://github.com/alex-wap/app-store/blob/master/images/1.png "App IDs")
* App ID Description can be anything. Under "Explicit App ID", **you must match your "Bundle ID" in Xcode.**
* Continue. Register.
* Click Provisioning Profiles - Distribution - Create new Provisioning Profile
![Provisioning Profile](https://github.com/alex-wap/app-store/blob/master/images/2.png "Provisioning Profile")
* Select **Distribution - App Store**. Continue.
* Select your App ID from the list. Continue.
* Select Certificate. Continue.
* Create Profile Name. Continue.
* Download Provisioning Profile and remember where it is.

## iTunes Connect
* Go to [iTunes Connect](https://itunesconnect.apple.com/). 
* Go to My Apps.
* Click the plus button to create a "New iOS App".
* Select iOS Checkbox.
* **Name field for your New App is permanent after submission. Pick what you want carefully.** 
* Select English for "Primary Language". 
* Select your Bundle ID. 
* SKU is a unique ID (you pick it). e.g. NameOfApp0.1
* Click Create

## iTunes Connect App Information
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