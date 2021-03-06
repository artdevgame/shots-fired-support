# Changelog

## 4.2.0 (28/01/2021)
* Reduced games to: Apex, CoD, CS:GO, Dota 2, Fortnite, Hearthstone,
  Heros of the Storm, LoL, Overwatch, PoE, PUBG, R6: Siege, Rocket
  League and Valorant
* Reduced events for each game
* Added a 'Reset app' button on the settings page that will remove any
  existing mappings for OBS or Webhooks

I'm currently working through the next version of Shots Fired but have
found it difficult to identify issues in the current version. By
reducing the games and events to ones that I can actively support I can
focus my efforts more onto v5.

I'm open to restoring games/events if there's something in particular
you'd like - just jump in the Discord group to let me know.
---

## 4.1.2 (18/01/2021)
Bug fixes:
* Protect against undefined.close call
* Protect against undefined.find call

New game events added
---

## 4.1.1 (20/11/2020)
* Bug fix: Some Overwolf events wasn't matching Shots Fired mappings due to the way the event data is structured. Updated the code to return the correct mapping based on a couple of conditions.
---

## 4.1.0 (06/10/2020)
- Users can see if they have a mapping on an event (icon)
---

## 4.0.3 (04/10/2020)
Bug fix:

* When adding a mapping, don't assume one exists
---

## 4.0.2 (04/10/2020)
* Corrects PUBG rank.me example
---

## 4.0.1 (03/10/2020)
Bug fixes:

* Updating a scene will cause the selected scene to reset, this prevents the app getting confused about scenes that no longer exist. 
* Saving an existing mapping for the second time won't reset the configuration unexpectedly


---

## 4.0.0 (01/10/2020)
* Introduces webhooks for further processing of game event data
* Adds Overwolf 'info' events
* Subscriptions are handled 100% by Overwolf again
* OBS connection details are input inline, rather than on a separate screen
* App is now more reactive to OBS
* New games supported (including Valorant & CoD)
---

## 3.1.0 (03/05/2020)
* Subscriptions are based on events rather than games
* Added the ability to gift Overwolf users a subscription
* Better handling of adding/removing scene items in OBS and reflecting in app
* Hotkey is now game specific rather than global
* Added Escape from Tarkov
---

## 3.0.0 (16/04/2020)
* The app has been totally rewritten to support more games, split over 2 tiers - free and premium. Premium tier requires an Overwolf subscription.
---

## 2.2.2 (03/05/2019)
* Adds PUBG trademark statement
---

## 2.2.1 (26/04/2019)
* Exposes app/store versions in the help screen and links through to the GitHub support repo.
* Overwolf only initialised once.
---

## 2.2.0 (26/04/2019)
* Tweaks based on best-practices, tech-review template and store submission docs
* App closes when game exits
* Help videos only available when connected to Internet
---

## 2.1.1 (22/04/2019)
* Control hotkeys from settings
* Adds a button to the help page to navigate to main screen
* Assets no longer stored in state
---

## 2.1.0 (22/04/2019)
* Versioning state changes
---

## 2.0.0 (22/04/2019)
* New UI
* Adds delay / duration form controls
---

## 1.2.0 (02/04/2019)
* Tracks errors through Sentry
---

## 1.1.0 (02/04/2019)
* First releasable version