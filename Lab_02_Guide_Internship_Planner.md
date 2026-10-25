<!--
STYLE GUIDE FOR THE LAB GUIDES (this comment doesn't appear in the preview)
- Headings: one # title per document; ## for main sections; ### for sub-steps.
- Heading capitalization: Title Case. Capitalize every word except short words (a, an, the, and, or, to, of, in, on, for, as, with) unless they come first.
- Bullets: * for top-level bullets, - for sub-bullets.
- Label bullets: start with a bold label and a colon.
- Things to click or press: bold, with the exact wording on screen.
- Commands: in a code block on their own line, never bold.
- Files, folders and email addresses: `code` style.
- Names: Claude desktop app, Cowork, MCP, Lab 00 / Lab 01 / Lab 02 / Lab 03.
- Images: centered <p align="center"> block with a width, one <br> before and after.
- Placeholders: [PLACEHOLDER - description] on its own line, with an empty line before and after.
- Punctuation: full sentences end with a period; no double spaces; use an em dash (—), not --.
- Spacing: one <br> (with empty lines around it) before each section heading, except the first.
- ENAS NOTE: students write their own prompts. The Answer Sheet is a rescue rope, not the path.
-->

# Lab 02 — Internship Discovery and Planner

*Track what's open, what you've applied to, and what's due next — in one place instead of six.*

## Introduction

This is the project where **you are the user**, which cuts both ways. You know exactly what's annoying about tracking internships, so you'll have strong opinions fast. The risk is building for yourself alone rather than for the five people at your table, who do it differently.

<br>

## Before You Start

* **One laptop, five people.** Decide who drives. The driver types; everyone else plans, watches the output and proposes what to try next. Swap if you like.

* **Your table's job is not to finish.** It's to get something real running and understand how you got there.

* **Laptops stay closed** until Step 02. The first thirty minutes are paper and pens — and that's the part that determines whether the build works.

<br>

## What You'll Build

A working page that holds the mess in one place:

* What's open, and when it closes.
* Where you are with each one.
* What needs doing next — and **something that acts on that**, rather than waiting for you to look.

<br>

## Step 01: Brainstorm Together — Laptops Closed

*About 30 minutes. Paper and pens on the table.*

Write your answers down. At the end of this step you'll hand what you wrote to Claude, so write it for a reader.

### Who Is This For?

* Compare how each of you tracks this today. Notes app, spreadsheet, memory, nothing?
* Where does it actually break down? Be specific about the last time it did.
* Whose version are you building? A first-year with no applications yet and a senior with twenty need different things. Pick one.

### What Does the Screen Show?

* Sketch it. One page, boxes and labels.
* What's the **first** thing you see when you open it on a bad Tuesday?
* A list, a calendar, a board, or something else? Argue about it, then decide.
* Name two things you're deliberately not building.

### Where Does the Data Come From?

* You will be given a set of internship postings to work with.

[PLACEHOLDER - how students connect to the workshop MCP server, once the server exists]

* What does a posting contain? Which fields matter enough to show?
* What does the student add themselves — status, notes, a rating?

### What Does It Do, Not Just Show?

*This is the agentic question, and the one worth most of your time.*

* A page that **displays** your applications is a spreadsheet with nicer fonts. What does yours **do**?
* Some directions worth arguing about:
    - It tells you what's due this week, without being asked.
    - It drafts the follow-up email to a recruiter who's gone quiet.
    - It notices a new posting that fits what you've already applied to.
    - It produces a calendar file for every deadline so they land in your real calendar.
* Pick **one**. Write down what triggers it, and what the result is.

<br>

## Step 02: Turn Your Notes into a Prompt

*Now the laptop opens.*

* **Open a Cowork session** connected to your project folder from Lab 00.

* **Two ways to get your plan in**, and the second is usually better:
    - Type it out.
    - **Photograph your notes** with a phone and attach the picture. Claude reads handwriting and sketches, and your sketch of the screen is usually clearer than a paragraph describing it.

* Write the prompt in your own words: who it's for, what the screen shows, where the data comes from, what it does.

<br>

## Step 03: Let Claude Interview You

*Optional, and recommended. Five minutes that saves twenty.*

> Before you build anything, interview me. Ask me five multiple-choice questions about what I want, one at a time. Then write a short plan as `MVP Plan.md` and show me a simple mockup with sample data. Wait for me to approve it before you write any other code.

This catches what your table forgot. It is also the lecture in miniature: you are directing an agent, not placing an order.

<br>

## Step 04: Build It

* Send your prompt.

* Claude will ask permission before it does things. **Click Allow** — or **Allow for this task** to reduce the clicking.

<br>

## Step 05: While You Wait

Builds take **ten minutes or more**. Plan for it.

* **Stay near the laptop.** Claude pauses to ask questions and waits until someone answers.

* **Non-drivers, you have work to do.** Discuss:
    - *Why is Markdown a useful language for configuring agents?*
    - Which of your five would actually use this next week? Why wouldn't the others?
    - What could go wrong if this had real deadlines in it and got one wrong?

* **Compare with your neighbors.**

<br>

## Step 06: Run It and Try It

* Claude will tell you how to start your app and give you a web address to open.

* Put in a real application you're tracking, or a plausible invented one. Does it hold up?

* Find one thing that's wrong or missing. That's your next prompt.

<br>

## Step 07: Add Your Own Twist

Whatever time is left is yours.

<br>

## If You Get Stuck

* **Strange file errors, or the build keeps failing:** check your project folder isn't in iCloud, Dropbox, OneDrive, Box or Google Drive. Move it to your home folder and try again.

* **Claude seems frozen:** look for a permission prompt waiting for a click.

* **The app won't start:** paste the error message back to Claude and ask it to fix it. This is normal.

* **You're out of ideas:** see the Answer Sheet below.

<br>

## Key Takeaways

* The thirty minutes on paper did more for your build than any single prompt.
* You directed an agent. It planned, used tools and acted — you decided what mattered.
* The gap between "displays information" and "does something" is the gap between an app and an agent.

<br>

## Answer Sheet

*Use these if your table is stuck. Reading them first spoils the exercise.*

[PLACEHOLDER - suggested prompts: a starting prompt, a prompt for adding the agentic action, and two recovery prompts for common failures]
