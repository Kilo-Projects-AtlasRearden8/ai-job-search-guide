STATUS — AI Job Search Guide
============================

What was built
--------------
A beginner-friendly manual and static HTML site for using AI in a job search.
Published by Asdale Dynamics, LLC (Indiana, formed October 2026).

Contents:
- LICENSE — MIT License, copyright line exactly "Copyright (c) 2026 Asdale Dynamics, LLC"
- README.md — project overview, chapter list, credit to Asdale Dynamics, LLC
- docs/ — Markdown manual, 7 plain-English chapters:
    1. getting-started.md — what AI is, how to write a prompt
    2. resumes.md — drafting and tailoring resumes with AI
    3. cover-letters.md — writing cover letters that sound like you
    4. interview-practice.md — practicing interview questions with AI
    5. application-tracking.md — keeping track of applications
    6. privacy-safety.md — what never to paste online
    7. cheat-sheet.md — ready-to-copy prompts
- site/ — static HTML version of the manual plus a browser-based tracker:
    - site/index.html — full manual in HTML with navigation
    - site/tracker.html — application tracker that saves only in browser localStorage
    - site/assets/style.css — shared styles for both HTML pages

No .github/workflows files were added. No build step is required; everything is static.

How to run it
-------------
- Read the Markdown manual: open any file in docs/ with a text editor or Markdown viewer.
- View the HTML site: open site/index.html in any web browser. Nothing needs to be installed.
- Use the tracker: open site/tracker.html in any web browser. Applications save to your browser's localStorage only — nothing is sent over the internet. Use the Export button to save a JSON backup; clearing browser data will delete saved applications.

Verification results
--------------------
- site/index.html: parses as valid HTML (no errors).
- site/tracker.html: parses as valid HTML (no errors).
- LICENSE line 3: exactly "Copyright (c) 2026 Asdale Dynamics, LLC".
- README.md credits Asdale Dynamics, LLC.
- Secret scan: no API keys, secrets, or personal data found (only privacy-warning mentions of the word "passwords").
- No .github/workflows directory present.

The tracker was functionally reviewed: add/delete/export/import flows are implemented in vanilla JavaScript with no external dependencies.

Known gaps
----------
- The Markdown docs and HTML site cover the same content but are maintained separately; edits to one are not automatically reflected in the other.
- The tracker has no user accounts or cloud sync (by design, local-first); data is tied to the browser and cleared if browser data is cleared unless exported.
- No automated test suite or linter is configured; the project is static HTML/Markdown with no build step.
- Content is educational writing help only and is not medical, legal, or career advice.
