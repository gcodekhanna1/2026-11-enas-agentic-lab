<!--
STYLE GUIDE FOR THE LAB GUIDES (this comment doesn't appear in the preview)
- Headings: one # title per document; ## for main sections; ### for sub-steps.
- Heading capitalization: Title Case. Capitalize every word except short words (a, an, the, and, or, to, of, in, on, for, as, with) unless they come first.
- Bullets: * for top-level bullets, - for sub-bullets.
- Label bullets: start with a bold label and a colon.
- Things to click or press: bold, with the exact wording on screen.
- Commands: in a code block on their own line, never bold.
- Files, folders and email addresses: `code` style.
- Names: Claude desktop app, Cowork, MCP, Streamlit, uv, Lab 00 / Lab 01 / Lab 02 / Lab 03.
- Images: centered <p align="center"> block with a width, one <br> before and after.
- Placeholders: [PLACEHOLDER - description] on its own line, with an empty line before and after.
- Punctuation: full sentences end with a period; no double spaces; use an em dash (—), not --.
- Spacing: one <br> (with empty lines around it) before each section heading, except the first.
- ENAS NOTE: one document. The discovery questions and the build steps live together here.
- ENAS NOTE: students write their own prompt. The Answer Sheet is a rescue rope, not the path.
-->

# Lab 02 — Internship, Discovery and Planner

*Thirty minutes describing the problem. The rest of the session building the answer.*

## The Goal

You're going after summer internships, and keeping track of it all gets overwhelming fast — which ones you care about, whether you've applied, who you've spoken to, what you owe them, and what you'd have to change in your resume.

You want one place that holds all of it.

<br>

## How Your Table Works

* **One laptop.** Decide who drives. The driver types; everyone else thinks, argues, watches the output and proposes what to try next. Swap whenever you like.

* **Everyone answers the questions.** The differences between you are the most useful thing on this page.

* **Your job is not to finish.** It's to get something real running and understand how you got there. Nobody expects a finished product in an hour.

<br>

## Step 01: Discovery — 30 Minutes

Work as a team to discuss the questions below. Feel free to add some of your own — these are just starters.

Remember that we are building and iterating. As a group, use your judgment for when you have done enough discovery to move on to building.

Write your answers down, or type them; you'll hand them to Claude at the end.

### Where Do You Normally Find Out About Internships?

Public job sites, the Yale career site, a professor, a friend who already works there?

### What Frustrates You Most About Applying?

Be specific. The last time it went badly, what actually went wrong?

### What Do You Wish You Could Remember About Each One — Before You Apply, and After?

Deadlines, links, who you emailed, where you stand, what they said.

### Are You Updating Your Resume / Cover Letter for Each Application? How?

### What Do You Find Out Too Late?

What are the things you want to be notified about?

<br>

## Look Back at What You Just Wrote. That's Your Portal.

You didn't design software. You described your own situation — and the thing you need falls out of it. Everything from here is construction.

<br>

## Step 02: Hand It to Claude

* **Open a Cowork session** connected to the project folder you made in Lab 00.

* Send Claude your answers along with this:

> Here are our notes on how we track internship applications, and what goes wrong.
>
> [paste your answers, or attach a photo of this page]
>
> Build us an initial minimum viable product that we can further customize working with you.
>
> Build it with:
> - Streamlit, in Python. Please don't use a different framework.
> - uv to install whatever it needs.
> - One start file, so we can run it again later with a single command.
> - A button that loads sample data, so we can see it working right away.
>
> Before you build anything: ask us up to five questions about whatever is unclear, then show us a mockup using sample data. Wait for us to approve the mockup before you write the real thing.

<p class="info"><b>Hint:</b> Claude handles images and photos as input very well. Photograph this whole page with a phone and attach it — handwriting, arrows, crossings-out and all. You don't need to type any of it out.</p>

<br>

## Step 03: Answer Its Questions, Then Judge the Mockup

* Claude will ask you a handful of questions. **Answer them as a table** — this is the part where the people not typing matter most.

* Then it shows you a mockup: a rough version with made-up data, before any real code exists.

* **Look at it properly.** Is this the thing you described? What's missing? What's there that nobody asked for?

* Say what's wrong and ask for another one. **Do not approve a mockup you don't like** — changing it now costs seconds, changing it after the build costs ten minutes.

<br>

## Step 04: Build It

* When the mockup is right, tell Claude to go ahead.

* Claude asks permission before it does things. Click **Allow**, or **Allow for this task** to reduce the clicking.

<br>

## Step 05: While You Wait

Builds take **ten minutes or more**. Plan for it.

* **Stay near the laptop.** Claude pauses to ask questions and waits until somebody answers. Nothing moves while it waits.

* **Everyone else, you have work to do.** Discuss:
    - *Why is Markdown a useful language for configuring agents?*
    - Which of your five would actually use this next week — and why wouldn't the others?
    - What could go wrong if this held real deadlines and got one wrong?

* **Compare with your neighbors.** The table next to you made different choices from the same questions.

<br>

## Step 06: Run It, Then Test It Properly

* Claude will tell you how to start your app and give you a web address to open.

* **Each of you add one real internship you'd actually go for.** Find the posting, paste the link. Five people, five different fields.

* That's the real test: does it work for the table, or only for whoever built it?

<br>

## Step 07: Make It Yours

Whatever time is left belongs to you. Fix the thing that annoyed you most in Step 06, or add the one feature somebody keeps asking for.

<br>

## If You Get Stuck

* **Strange file errors, or the build keeps failing:** check your project folder isn't in iCloud, Dropbox, OneDrive, Box or Google Drive. Move it to your home folder and try again.

* **Claude seems frozen:** look for a permission prompt waiting for a click.

* **The app won't start:** paste the error message back to Claude and ask it to fix it. This is normal and expected — it is not a sign you did something wrong.

* **You're out of ideas:** see the Answer Sheet at the bottom.

<br>

## Key Takeaways

* **The thirty minutes of talking did more for your build than any single prompt.** You described a problem; the design came out of the description.

* **You reviewed a plan before accepting the work.** That one habit separates people who get good results from people who get impressive-looking ones that break.

* **You directed an agent.** It asked, planned, used tools and built — you decided what mattered.

* **A thing that displays is a page. A thing that acts is an agent.** Question 5 is where yours crossed that line.

<br>

## Answer Sheet

*Use these if your table is stuck. Reading them first spoils the exercise.*

[PLACEHOLDER - suggested prompts: a worked starting prompt, a prompt for adding the agentic action, and two recovery prompts for common failures]

<br>

## What's Next

Your app lives in your project folder. Share it with your table, keep building, or start something else entirely — you now know how.
