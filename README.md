# CAPABLE iPhone App

This is a static Progressive Web App (PWA). It has no server, account, or database requirement.
Progress is stored locally on the iPhone in Safari/Home Screen storage.

## Fastest setup: GitHub Pages

1. Create a new GitHub repository, for example `capable-app`.
2. Upload everything inside this folder to the repository root.
3. In GitHub, open **Settings > Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Choose **main** and **/(root)**, then Save.
6. GitHub will show a Pages URL after deployment.
7. Open that URL in **Safari on the iPhone**.
8. Tap **Share > Add to Home Screen**.

After the first load, the service worker caches the app so it can continue working offline.

## What the app does

- Asks how much time you have.
- Filters by activity type and location.
- Uses the 318 skills from `CAPABLE_Field_Guide_With_Challenges.xlsx`.
- Shows Why It Matters and the Safety Note as "The wiser way."
- Lets you save ideas.
- Lets you mark skills done and record rating, independence, and a short reflection.
- Includes Quick Capture for new ideas life reveals.
- Exports progress as CSV and backs up app data as JSON.

## Updating the skill library later

This version has the current CAPABLE skill list embedded in `index.html`.
When the spreadsheet changes substantially, regenerate the app from the workbook or replace the embedded `SKILLS` array.

## Privacy

There is no analytics and no cloud storage in this build. Saved ideas, completed skills, notes, and captures live in the browser's local storage unless you export them.
