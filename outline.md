# An Outline of the app for internal use

## Purpose
Get notifications whenever a push is made to a particular github repo.
Also FUCK WINDOWS. Only for linux + mac.

## Flow outline
List all repos that you are contributing to.
Each repo has 3 options
- shh!
- periodical (default time of 1 min)
The app will live in the native OS tray

## Programming Outline

### UI
Sync Button.
List of all repos.
Each list item comes with:
- Name of the repo
- Latest Commit (200 chars)
- Latest Committed filename
- Latest Commit author
- icon to shh!
- icon to set period
- icon for predominant language
Status bar within app to tell us if it is fetching from github, connection down etc...
Notification area in app with a clear button
Show me the code button which takes you to that commit on github

### LOGIC
- Open the app
- Displays from local db
- Refreshes in background
  - Sends latest stored commit and checks if there is a new commit for each app
- Shows shit if app in focus else notify