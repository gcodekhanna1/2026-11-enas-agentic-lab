<!--
STYLE GUIDE FOR THE LAB GUIDES (this comment doesn't appear in the preview)
- Headings: one # title per document; ## for main sections; ### for sub-steps.
- Heading capitalization: Title Case. Capitalize every word except short words (a, an, the, and, or, to, of, in, on, for, as, with) unless they come first.
- Bullets: * for top-level bullets, - for sub-bullets.
- Label bullets: start with a bold label and a colon.
- Things to click or press: bold, with the exact wording on screen.
- Commands: in a code block on their own line, never bold.
- Files, folders and email addresses: `code` style.
- Names: Claude desktop app, Cowork, MCP, Streamlit, uv, Lab 00 / Lab 01 / Lab 02.
- Images: centered <p align="center"> block with a width, one <br> before and after.
- Punctuation: full sentences end with a period; no double spaces; use an em dash (—), not --.
- Spacing: one <br> (with empty lines around it) before each section heading, except the first.
- ENAS NOTE: the prompts behind Lab 01's "Need a Nudge?" link (was the Answer Sheet, moved here 11/17). Not listed on the landing page.
-->

# Lab 01 — Prompt Ideas

*Prompts other tables have tried. Borrow an idea, change it to fit what your table wants, and keep your own voice.*

* **A worked starting prompt,** for a table that keeps missing deadlines:

> We're a table of Yale sophomores applying to summer internships in finance and consulting. Each of us is tracking 10 to 20 applications across job sites, the Yale career site and emails from recruiters, and we keep missing deadlines and forgetting who we talked to. When we open the planner, we want to see in five seconds what's due this week and what we're waiting to hear back on. Build us an initial minimum viable product: one page with the next deadlines at the top, then a list of every internship with its company, role, deadline, link, contact and status, and a form to add a new one. Use Streamlit, in Python, with uv, one start file, and a button that loads sample data. Ask us up to five questions first, then show us a mockup and wait for our approval.

* **Making it act on its own deadlines:**

> Add a "Remind Us" button next to each internship. When we click it, send a reminder about that internship with a calendar invite three days before its deadline, through the workshop server's send_reminder tool, to our table's lab account. Show us a message saying whether it was sent. Don't send real reminders while you test; we'll send the first one ourselves.

* **The reminder button doesn't send anything:**

> The reminder didn't arrive. Show us the exact error, or the server's reply if there was no error. Then check: the address ends in /mcp, the access key is read from our settings file, the lab account is demo-XX@paradigmventures.ai, and the code uses the current version of the official `mcp` library. Change one thing at a time and tell us what you changed.

* **Claude keeps tuning and nothing changes on screen:**

> Stop here. Give us the simplest version that works right now, restart the portal, and tell us what to click to see it. We'll decide what to improve next.

<br>

[← Back to Lab 01](Lab_01_Guide_Internship_Planner.html)
