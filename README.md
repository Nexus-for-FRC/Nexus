# 📢 [FRC Queue](https://www.frcqueue.com)
A web-based queuing system with SMS notifications designed to solve common queuing pain points.

**Current status**: Updated version available for offseason events

## Bugs/Feature requests
[File issues here](https://github.com/frc-queue/frc-queue/issues/new) to report bugs or request new features.

## Change log
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
