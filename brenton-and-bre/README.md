# Brenton & Bre’s wedding countdown

A responsive wedding page with a live countdown, month calendar, date calculator, and downloadable calendar event. No build tools or account keys required.

## Put it live on GitHub Pages

1. Create a GitHub repository (for example, `brenton-and-bre`). Use a public repository if you want free GitHub Pages hosting.
2. Upload `index.html` and `.nojekyll` to the repository’s top level. Do not upload the ZIP itself.
3. Open the repository’s **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**, then **main** and **/ (root)**. Save.
5. GitHub will show the published address on that screen after deployment, typically `https://YOUR-USERNAME.github.io/brenton-and-bre/`.

## Wedding date and time

The page uses **April 17, 2026 at 2:00 p.m. America/Chicago** as requested. Since this date has passed, it shows elapsed time since the ceremony. Future dates automatically show a countdown.

To set a different year for every visitor, edit this line in `index.html`:

```js
const WEDDING_DATE = '2026-04-17';
```

The following two lines control the ceremony time and time zone. Daylight saving time is handled automatically.

```js
const WEDDING_TIME = '14:00';
const TIME_ZONE = 'America/Chicago';
```

If you change the date, also update the description near the top of the file. The on-page date adjustment is a temporary preview; it does not change the source on GitHub.

The main timer measures exact elapsed time. The calculator measures calendar days. “Save the date” downloads a calendar entry with the ceremony start time and a one-hour placeholder duration; no wedding end time or venue has been supplied.

The page uses Google Fonts when available, with local font fallbacks. Everything else is included in `index.html`.
