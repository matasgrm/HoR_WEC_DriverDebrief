Heart of Racing / AMR – WEC Driver Debrief
Mobile-friendly post-event driver feedback form for Heart of Racing / Aston Martin Racing.
Current event version: Monza 2026
The form is designed to run as a static website on GitHub Pages and works on iPhone/iPad Safari, Android, Chrome, Edge and desktop browsers.
Live site
If this repository is published from the `main` branch and repository root, the site address is:
https://matasgrm.github.io/HoR_WEC_DriverDebrief/
Files
`index.html` – the complete driver debrief app. The styling, track map, logic, local saving, balance calculations and engineer-email generation are all contained in this file.
`README.md` – these GitHub Pages instructions.
No build process, server or package installation is required.
First-time GitHub Pages setup
Open the GitHub repository.
Go to Settings.
Select Pages in the left-hand menu.
Under Build and deployment, set Source to `Deploy from a branch`.
Select branch main.
Select folder /(root).
Click Save.
GitHub will publish the site automatically.
The repository must contain `index.html` at the top level, not inside another folder.
Updating the debrief for a new event
Normally only `index.html` needs to be replaced.
Download the new `index.html` supplied for the event.
Open this GitHub repository.
Click Add file → Upload files.
Drag the new `index.html` into the upload area.
GitHub will recognise that an `index.html` already exists and replace it when the change is committed.
Add a short commit message, for example `Update driver debrief for Monza`.
Click Commit changes.
GitHub Pages will redeploy automatically. There is normally no need to republish the site manually.
Allow a short period for GitHub Pages to update, then reload the normal website address.
Browser cache / old event still showing
The form stores an unfinished debrief locally in the driver's browser so work is not lost if Safari or Chrome is closed.
Each event uses a separate storage key. This prevents a previous event's answers from appearing in the next event.
If an old version of the webpage itself is still visible after an update:
close the old browser tab and reopen the website link;
on desktop, use a hard refresh (`Ctrl + F5` on Windows);
on iPhone/iPad Safari, close the tab and reopen the GitHub Pages link.
The Clear button removes the saved draft for the current event only.
Driver workflow
Open the GitHub Pages link in Safari or another browser.
Select driver and car number.
Complete session feedback. Use N/A if the driver did not take part in a session.
Tap through OK / Issue / N/A in Car Feedback. Add a short comment only where useful.
Complete the balance sliders for the Monza corner groups.
Add weekend conclusions.
Scroll to the bottom and press Send to Engineers.
No app, TestFlight installation or login is required.
Monza balance groups
The Monza balance debrief uses the following references:
T1–2 – Chicane 1
T3 – Curva Grande
T4–5 – Chicane 2
T6 – Lesmo 1
T7 – Lesmo 2
T8–10 – Ascari
T11 – Parabolica
Each group has separate Brake / Turn-in / Mid / Exit sliders from `US5` through `Neutral` to `OS5`.
Send to Engineers
The form automatically prepares the engineer email for:
`mgrigalauskas@prodrive.com`
`ewarnett@prodrive.com`
The email automatically includes the event, date, driver, car, session feedback, grouped car-feedback subsections, calculated balance overview, highest-severity corner groups, detailed corner balance and driver conclusions.
On mobile, Send to Engineers opens the device's default mail flow.
On laptop/desktop, the form offers:
Gmail Web
Outlook Web
Default Mail App
Copy Full Email
This avoids relying on Outlook being installed locally.
Privacy and data storage
The static GitHub Pages version does not use a database. Draft answers are stored only in the browser's local storage until they are cleared. The email is generated on the device when the driver presses Send to Engineers.
Important when creating the next event version
When changing the event, update all of the following in `index.html`:
event/circuit name;
embedded track map;
balance corner/group list and names;
event-specific wording in the engineer summary;
local-storage key so previous-event drafts cannot carry across.
Example storage key format:
`hor_monza_2026_driver_debrief_v1`
Use a new unique key for every event.
