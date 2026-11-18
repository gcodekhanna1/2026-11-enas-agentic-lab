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
- ENAS NOTE: the prompts behind Lab 02's "Need a Nudge?" link (was the Answer Sheet, moved here 11/17). Not listed on the landing page.
-->

# Lab 02 — Prompt Ideas

*Prompts other tables have tried. Borrow an idea, change it to fit what your table wants, and keep your own voice.*

* **A worked starting prompt,** for a table building for first-time investors:

> We're a table of Yale students building a stock tracker for a student who has just invested their first $500 and checks it on their phone between classes. When they open it, they want to know in five seconds: am I up or down today, and why? They don't want charts full of numbers, and they never want to be told what to buy or sell. Build us an initial minimum viable product: one page with the total value and the day's change at the top, then each holding with its change and a one-line reason. Use Streamlit, in Python, with uv, one start file, and sample data for a few well-known stocks we can change. Ask us up to five questions first, then show us a mockup and wait for our approval.

* **The portal can't get data from the workshop server:**

> Our portal can't get data from the workshop server. Show us the exact error. Then check: the address ends in /mcp, the access key is read from our settings file, and the code uses the current version of the official `mcp` library. Make one call to get_live_quote for AAPL and show us the result before changing anything else.

* **Claude keeps tuning and nothing changes on screen:**

> Stop here. Give us the simplest version that works right now, restart the portal, and tell us what to click to see it. We'll decide what to improve next.

* **The explanation doesn't match the news (mock portfolio):**

> The explanation for [company] doesn't match the headline. Show us the price change and the headlines you used, then only explain a move when a headline from get_news matches the company and the day. Otherwise say there's no news for it.

<br>

[← Back to Lab 02](Lab_02_Guide_Portfolio_Tracker.html)
