# [Nexus for FRC](https://frc.nexus)

A web-based event management system designed to improve the team experience at FRC events.

## Bugs/Feature requests
[File issues here](https://github.com/frc-queue/frc-queue/issues/new) to report bugs or request new features.

## Change log
### 2025 Preseason- February

#### Inspection
- Updated inspection checklist to 2025v1

#### Backup teams
- When adding backup teams to an alliance on the alliances page, lead queuers can now optionally send a notification to the affected team

### 2025 Preseason- January

#### Announcement notifications
- Teams can now opt in to recieve Slack or Discord notifications for event announcements and parts requests. The parts requests system will be available at all events.

#### Inspection
- Bumper weight input interface updated to support 2025 weight limits

#### Pit display
- Added announcements and parts requests carousel to pit display during playoffs

### 2024 Offseason- December

#### Pick-a-pit
- Pick-a-Pit is a system that allows teams to select their pit location for a specific event. Access can be prioritized to provide a team incentive, for example, to encourage volunteering. Pick-a-Pit was trialed in Northern California for the 2024 season and is now available for any event. Select "Pick-a-pit" in the volunteer menu for your event to get started.

#### The Map Update
- Added Pit Mapper (beta) tool that allows volunteers to design pit maps that can be viewed by volunteers and teams at the event
- Added pit assignment interface to allow volunteers to assign teams to specific pit locations
- Added option to view inspection progress as a map
- Custom team checklists (created on the teams page) can now be viewed as a map
- Teams can view the pit map and search for specific teams

![Inspection map](https://github.com/user-attachments/assets/e83b5b62-940b-4da6-ae4e-586f69e718e8)


### 2024 Offseason- November

#### Inspection
- Added "Start playoff reinspection" button on the LRI requests page. All teams can be flagged for a playoff reinspection with a single tap on the LRI requests page. Tap this button on the last day of the event, prior to the last round of qualifications. Every team that completed their initial inspection will be moved to the "Waiting for inspector" section. Teams will be sorted chronologically by their last qualification match, so they can be quickly processed in order.

### 2024 Offseason- September

#### Inspection
- Added "on hold" state for in-progress inspections that do not currently require attention from inspectors
- Added log page to view the full history of inspection actions for a specific team
- Added checking of inspection items from the full checklist view (useful for inspectors who prefer to check items in arbitrary order)
- Added manual inspector assignment/unassignment buttons. Inspector assignment still happens implicitly when certain actions are taken, but in some cases the explicit assignment may be useful
- Added option to manually move a "not started" team to "waiting for inspector". This is useful for venues that don't support the inspection process that begins with weigh-in
- Weight values are now displayed in the main checklist view
- Weight values can now be entered and displayed in metric by tapping the units next to the input fields
- If a team is scheduled in an upcoming match, it will be displayed on the team's inspection page
- Added reinspection for items that require inspector attention after a team's initial certification
  - Teams can request reinspection themselves by scanning their Nexus code, tapping "Request reinspection" and filling out the form
  - FTAs can request reinspection for teams from the FTA notepad
  - Inspectors can flag teams for reinspection from the team's inspection page
- An inspector Slack channel can now be connected on the LRI requests page. The channel will receive a message anytime:
  - An inspector flags a checklist item for the LRI
  - An inspector flags a team for reinspection
  - An FTA flags a team for reinspection
  - A team requests reinspection by scanning their Nexus code and filling out the form
- A notification will now be sent to each team when their inspection is certified (if they have registered for notifications)
  - The message will include a reminder of the reinspection rule

### 2024 Offseason- June

#### API
- Added public API v1.1.0 which allows developers to use live event status data and match timing estimates in their own applications

#### Queuing
- Implemented "slide to queue" for touchscreen devices to reduce mistaken taps
- Updated queue timing tooltip to include detailed timing for each match. This can now be viewed when hovering over the match status chip on the main queuing screen
  - Estimated times will be shown for future status changes (with tilde)
  - Actual times will be shown for past status changes
  - Scheduled match start time will be shown if available
- Improved protection against accidental double queuing. A warning will now be shown if *any* user has updated a match status within the past 4 minutes. Select the confirmation checkbox to bypass the warning and queue anyway.
- Added underline in the filler team selection dialog if a team has not played in any matches yet
- Added "unset winner" option for playoff matches, in case of an accidental selection or late replay announcement
- Added schedule behind/ahead indicator to queuing dashboard header
- Added "Create filler match" button to the main queuing screen during practice matches

#### Teams list page
- Minor changes to simplify the teams table 
- Added column to indicate if each team has played in a match
- Added ability to create custom team check-off columns for arbitrary tracking of teams

#### Volunteer menu
- The new "volunteer menu" improves the navigation experience between event volunteer pages
- Added link to the "Nexus Support" Slack workspace
- Added a yellow badge on the volunteer menu that is shown when there are actionable requests (user access requests, pending parts requests, and LRI requests)

#### Displays
- Added schedule behind/ahead indicator to pit display
- Added "audience" display to show the next few upcoming matches including team numbers
- Added simple "queuing" display to show the match that is currently on field and any upcoming matches that are on deck or now queuing


#### Misc
- Added "Playoff type" setting
   - View [all bracket options here](https://github.com/Nexus-for-FRC/Nexus/blob/main/playoffs.md)
- Added keyboard shortcuts:
  - FTA Notepad: 
      - Previous `,`
      - Next `.`
      - Current `/`
  - Queuing: Scroll to now `/`
  - Scorekeeper: Scroll to now `/`


### 2024 Offseason- May
- Added QR-code based volunteer onboarding flow to the user & inspector management pages
- Added option to grant additional roles to existing users on the user management page
- Updated inspection checklist to 2024v3
- When manually importing matches, blue teams are now on the left. The team order now matches the FMS match report.

<details>
   <summary>
     <h3>Older changes</h3>
   </summary>

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
