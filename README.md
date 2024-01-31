## Flask Application Design: Cricket Scorecard
----
### HTML Files
- **index.html**:
   - This is the homepage of the application that displays a list of local cricket teams.
   - It includes a link for each team to its respective scorecard page.

- **scorecard.html**:
   - This page displays the scorecard of a particular team.
   - It includes a table to show the team's name, total runs, wickets, and other relevant statistics.
   - There is also a section to add new entries to the scorecard, such as runs, wickets, and player names.

### Routes
- **Homepage**:
   - Route: `/`
   - Function: Displays the index.html page, which lists all the local cricket teams.

- **Scorecard Page**:
   - Route: `/scorecard/<team_id>`
   - Function: Displays the scorecard.html page for a specific team, where `<team_id>` is the unique identifier of the team.

- **Add Entry**:
   - Route: `/add_entry`
   - Function: Adds a new entry to the scorecard of a specific team.
   - This route receives data from the scorecard.html page when a user adds a new entry, and it updates the scorecard accordingly.

- **Update Score**:
   - Route: `/update_score`
   - Function: Updates the total runs or wickets on the scorecard.
   - This route receives data from the scorecard.html page when a user updates the score, and it updates the scorecard accordingly.

- **Delete Entry**:
   - Route: `/delete_entry`
   - Function: Deletes an entry from the scorecard of a specific team.
   - This route receives data from the scorecard.html page when a user deletes an entry, and it removes it from the scorecard accordingly.