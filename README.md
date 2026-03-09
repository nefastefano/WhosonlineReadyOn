:::writing{variant=“standard” id=“48261”}

Coverage Checker

Coverage Checker is a simple web app that provides a quick view of who is currently working across a distributed team.

It helps teams quickly understand availability across time zones without needing to manually check schedules.

The app shows:
	•	Who is currently online
	•	Who will come online in the next 24 hours
	•	Who will be online at the same time tomorrow
	•	Who is currently out of office (OOO)

How it works

The application reads schedule data from a Google Sheet and calculates availability dynamically based on each person’s time zone and working hours.

All calculations are performed directly in the browser using JavaScript. No backend or server is required.

Because time zones are handled per person, the coverage calculation works well for globally distributed teams.

Data source

Availability data is maintained in a shared Google Sheet.

Typical fields include:
	•	name
	•	tz
	•	days
	•	start
	•	end
	•	First day OOO
	•	Last day OOO
	•	Team

The application reads the spreadsheet through a published CSV endpoint.

Team members update their working schedule directly in the spreadsheet.

Features
	•	Real time availability overview
	•	Automatic time zone handling
	•	Visibility of shifts starting within the next 24 hours
	•	Tomorrow’s availability preview
	•	Out of office tracking
	•	Optional team filtering
	•	No backend required
	•	Runs entirely in the browser

Deployment

The application is hosted using GitHub Pages via this repository.

Because it is a static application, deployment simply requires updating the repository.

Typical workflow:
	1.	Update the index.html file if changes are needed
	2.	Commit and push the changes to the repository
	3.	GitHub Pages will automatically update the live site

Usage
	1.	Open the application in a browser.
	2.	The schedule will load automatically from the Google Sheet.
	3.	Optionally select a specific team using the team filter.

The page will display:
	•	People currently working
	•	People coming online soon
	•	Tomorrow’s availability
	•	Out of office information

Updating schedules

Team members should update their working hours and time off directly in the shared Google Sheet.

Changes will automatically be reflected in the application.

Support

For issues or enquiries about this app, feel free to reach out to Ste.
:::
