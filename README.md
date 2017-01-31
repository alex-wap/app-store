# How-to Guide for Apple App Store Submittal


## Prerequisites
* [Apple Developer Account](https://developer.apple.com/)
* [Sign up for Apple Developer Program](https://developer.apple.com/account/#/membership/)
* **Screenshots**. You can generate these using the Simulator and Command+S to take a screenshot. **You must use Window > Scale > 100% (Command+1)**
  * **REQUIRED** one iPad Pro screenshot.
  * **REQUIRED** one iPhone 7 Plus screenshot. 
  * These are the highest resolutions for iPad and iPhone.
* **1024px X 1024px Image** (your App Icon as JPG).
* Add App Icons to your project.
  * Go to Project - General - App Icons and Launch Images - App Icons Scource.
  ![app icons](https://github.com/alex-wap/app-store/blob/master/images/0.png "app icons")
  * Use Asset Catalog or create a new one.
  * Open assets folder in your project.
  * Use a Mac App [Prepo](https://itunes.apple.com/us/app/prepo/id476533227?mt=12) or make your own icons ([Gimp](https://www.gimp.org/downloads/) or [Pixlr](https://pixlr.com/editor/)). 
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
  * Drag and drop your icons from the Finder into the assets folder in Xcode. **if your icons are in "CarPlay", move them to iPhone App 60pt.**
  * Your AppIcon layout should look like the screenshot below:
  ![appicon page](https://github.com/alex-wap/app-store/blob/master/images/appicon.png "appicon page")
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
* Category is required.
* Click Save (top right corner)
* Click Yellow "1.0 Prepare for Submission" on the left sidebar.
![Prepare for Submission](https://github.com/alex-wap/app-store/blob/master/images/prepareforsubmission.png "Prepare for Submission")

## iOS App 1.0 Prepare for Submission
* Choose File > Your iPhone screenshot from the prerequisite section. 
* Click iPad button above screenshot preview.
* Choose File > Your iPad screenshot from the prerequisite section. 
* Click Save (top right)
* Description is required. 
* Keywords are required. 
* Support URL is required (your website or github). 
* Ignore "Build" for now and scroll down to "General App Information".

## General App Information
* App Icon > Choose File > Your 1024x1024px icon from prerequisite section.
* Click edit next to "Rating". Fill out questionnaire. Be careful, **it's easier to get approved if you don't select "Made For Kids".** Click Done.
* Copyright (your business name) required.
* Address information is required.

## App Review Information
* Fill out contact information for "App Review Information"
* You do not need a "Demo Account". Uncheck the box.
* Select "Automatically release this version".
* Click the Save button in the top right.
* Click Pricing and Availability in the top left corner.

## Pricing and Availability
* Select Price Tier "Free".
* Save.
* Click Yellow "1.0 Prepare for Submission" on the left sidebar.
* Switch to Xcode.

## Xcode
* Select your build target as "Generic iOS Device"
![build target](https://github.com/alex-wap/app-store/blob/master/images/3.png "build target")
* From the Top Menu Bar, Select **Product > Archive**
![archive](https://github.com/alex-wap/app-store/blob/master/images/4.png "archive")
* After Archiving successfully, a window will open with your archive.
* Find your Provisioning Profile file (most likely in your Downloads Folder) and double-click it from your Finder.
* Xcode will open the file.
* Click Validate. Choose Development Team. Loading Screen. Click Validate again.
* Wait for "Validation Successful". (long wait) Click Done.
  * Most errors will occur at this stage. Read the error messages and check Stack Overflow for solutions if they are not obvious.
* Click "Uplaod to App Store...". Select your Development Team. Click Choose.
* Click Upload. (long wait)
* Switch back to [iTunes Connect](https://itunesconnect.apple.com/).

## [iTunes Connect](https://itunesconnect.apple.com/)
* Reload the iTunes Connect page showing your app.
* Your build may take several minutes to process before it will be available on the page.
* Scroll down to "Build" and the plus icon will show up next to "Build". Wait and refresh the page if it is not there yet.
* Click the plus button. Add Build. Click Done.
* Save. Submit for Review. Follow instructions if you're missing information.

## Export Compliance, Content Rights, and Advertising Identifier
* Select "No" for Export Compliance
* Select "No" for Content Rights
* Select "No" for Advertising Identifier.
* Click Submit.

## Congratulations!
* App is now "Waiting For Review". 
  * The next stages are:
  * "Preparing for Review"
  * "Going in Review"
  * "Accepted" or "Rejected" 
* You will receive an email for your app's approval, but it is good to check it yourself in [iTunes Connect](https://itunesconnect.apple.com/).

## Live Demo of Apple App Store Deployment


**Coming Soon**


## Alternative Video


[Slightly Outdated - Jared Davidson - Submitting an App to the iOS App Store](https://www.youtube.com/watch?v=6uX7B8ZfMiw)