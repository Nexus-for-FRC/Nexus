# [Nexus for FRC](https://frc.nexus)

A web-based event management system designed to improve the team experience at FRC events.

**Current status**: Available for 2024 offseason events

## Bugs/Feature requests
[File issues here](https://github.com/frc-queue/frc-queue/issues/new) to report bugs or request new features.

## Change log
### 2024 Offseason- May
- Added QR-code based volunteer onboarding flow to the user & inspector management pages
- Added option to grant additional roles to existing users on the user management page
- Updated inspection checklist to 2024v3
- When manually importing matches, blue teams are now on the left. The team order now matches the FMS match report.
- Queuers can now see the scheduled start time for each practice & qualification match by tapping the match name
<img src="https://github.com/Nexus-for-FRC/Nexus/assets/2548822/8195b1ec-c39e-44f7-81b1-b3b4c3ec8682" alt="Scheduled match time" width="300"/>

### 2024 Week 2


#### Turkish
- All team-facing UIs are now available in Turkish. Use the selector in the footer to override the default language.
  - Thanks to Oğuzhan!

### 2024 Week 0
-  Updated inspection checklist to 2024v2

### 2024 Preseason- February
-  Updated inspection checklist to 2024v1

### 2024 Preseason- January
-  Disabled ability for queuers to enter playoff lineups for official events
-  Added volunteer walkthrough videos for [FTAs](https://frc.nexus/en/guide/fta), [lead queuers](https://frc.nexus/en/guide/lead-queuer), [LRIs](https://frc.nexus/en/guide/lri), and [pit admin](https://frc.nexus/en/guide/pit-admin)
-  "Enable queuing extra match" option removed from settings- email contact@frc.nexus to enable this for your event
-  Now accepting translation contributions for Hebrew, Turkish & Portuguese. View the [translations documentation](translations.md) for details on how to contribute
-  Added the ability to export inspection data as a CSV

<details>
   <summary>
     <h3>Older changes</h3>
   </summary>

  ### 2023 Offseason- September
  
  #### Playoffs
  -  The [2024 playoff schedule](https://www.firstinspires.org/robotics/frc/blog/2023-double-elimination-2023-data-and-updates) is now used by default, with no breaks between rounds 1, 2, and 3. Prefer to use this schedule at offseasons whenever possible.
  
  #### Spanish
  -  All team-facing UIs are now available in Spanish. Use the selector in the footer to override the default language.
     -  Thanks to Ivan, Alejandro, Fermin from FRC teams [6017](https://www.thebluealliance.com/team/6017) & [7421](https://www.thebluealliance.com/team/7421)!
  
  ### 2023 Offseason- August
  
  #### FRC Queue is now "Nexus for FRC"
  -  Updated URL to [frc.nexus](https://frc.nexus)
  
  #### Inspection tools (BETA)
  -  Added tools for LRIs and inspectors to track inspection status of robots at events
  
  #### Demos
  -  Demo events are now available from the [events page](https://frc.nexus/events)
  
  #### Documentation
  -  Updated event and volunteer guides are now published
  
  
  ### 2023 Offseason- July
  
  #### Updated queuing workflow
  - Queuing action buttons are now at the bottom of the screen instead of next to each match
  - Updated guidance to queue the next match when scores are posted instead of when the field reset signal is given
  - Simplified playoffs queuing significantly- winner selection is now on the main screen and will automatically trigger the next queuing action
    - A new queuing sequence is implemented to maintain notification consistency (matches should be queued ~15 minutes before the teams need to be on the field)
    - This will automatically queue the next playoff match at the right time, even taking breaks into consideration
  
  #### Added dedicated scorekeeper view 
  - Optimized for reading lineups for practice & playoff matches 
  
  #### Misc
  - Updated team handouts (now 3 per page)
  - Added playoff bracket to queuing screen
  - Moved alliance selection check-off to the main queuing screen
  
  ### 2023 Offseason- May
  
  #### Updated queuing dashboard
  - Combined schedule management functionality into main queuing dashboard
  - All matches can be viewed from the main queuing screen (with button at the top to scroll to the current match)
  - Added ability to queuers to enter in playoff lineups
  - Added automatic imports of qual schedules & playoff alliances
  
  #### Updated team dashboard
  - Shows more information about a team's upcoming matches
  - Shows event announcements, parts requests, and the technical help request form
  - Added Discord option for queuing notifications
  
  #### New pit display
  - Designed for large screens & TVs
  - Displays queuing status, event announcements, parts requests and rankings
  
  #### New authorization system
  - Supports more fine grained roles (Admin, Lead queuer, Queuer, Pit admin, Field tech)
  - Supports "device accounts"- grant access to specific devices without needing to login to a Google account
  - New access request form makes it easier to onboard volunteers at events
  
  #### Misc
  - Added interface for pit admin volunteers to review and submit announcements
  - Overall UX refresh
  - Added light theme
  
  Updated documentation & demo events coming soon

   ### 2023 Week 6 (v209)

   - Updated icons and style for team check-in status to improve contrast
   - Green check: fully checked in
   - Yellow person: Human member of drive team checked in, but no robot
   
   ![Updated icons](https://user-images.githubusercontent.com/2548822/229666756-e032dcfd-b75a-44c4-96f6-8e38715786f7.png)
   
   ### 2023 Week 2 (v197) 
   
   - Updated team phone number input field to include country selector. Team members with non-US phone numbers can either select their country with the flag dropdown or manually enter their country code preceeded by a `+`.
   
   ![Phone number country input](https://user-images.githubusercontent.com/2548822/223203303-a70dbc2f-0df6-421c-a1ad-7fea251944f5.png)
   
   - Team representatives for alliance selection can now be requested a bit sooner via the Tasks panel (once the last qual match is queued). While announcements can be made before this to remind teams they will need to send their representative by the end of qualifications, actually asking representatives to come to the field should not happen too early as teams are busy strategizing and making a student stand near the field for 30+ minutes is unnecessary
   - Single match queuing- if your venue does not have enough space to queue two matches deep (both "on deck" and "now queuing"), you can turn on the "Enable single match queuing" setting. This will disable the "Advance queue" functionality so you can individually queue matches. Each match will still have both "Now queuing" and "On deck" states, so you can send a slightly earlier notification and a final reminder.
   - Bug fix for date-time input fields that made it difficult to enter times on some devices
   - Added a button to clear a team from a playoff alliance, in case they were accidentally added as a backup team
</details>
