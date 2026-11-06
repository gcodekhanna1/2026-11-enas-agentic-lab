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
- Placeholders: <p align="center" style="color:#800000"><b>[PLACEHOLDER - description]</b></p> on its own line, with an empty line before and after. Delete it when the content is added.
- Punctuation: full sentences end with a period; no double spaces; use an em dash (—), not --.
- Spacing: one <br> (with empty lines around it) before each section heading, except the first.
- ENAS NOTE: one document. The discovery questions and the build steps live together here.
- ENAS NOTE: students write their own prompt. The Answer Sheet is a rescue rope, not the path.
-->

# Lab 01 — Internship, Discovery and Planner

*Thirty minutes describing the problem. The rest of the session building the answer.*

## The Goal

You're going after summer internships, and keeping track of it all gets overwhelming fast — which ones you care about, whether you've applied, who you've spoken to, what you owe them, and what you'd have to change in your resume.

You want one place that holds all of it.

<br>

## Step 01: Brainstorming and Discovery

*About 30 minutes, as a guide rather than a limit.*

Work as a team to discuss the questions below. Feel free to add some of your own — these are just starters.

Remember that we are building and iterating. As a group, use your judgment for when you have done enough discovery to move on to building.

Capture your answers on your template, whiteboard and sticky notes. You'll photograph them and hand them to Claude at the end.

* **Where Do You Normally Find Out About Internships?**
    - Public job sites, the Yale career site, a professor, a friend who already works there?

* **What Frustrates You Most About Applying?**
    - Be specific. The last time it went badly, what actually went wrong?

* **What Do You Wish You Could Remember About Each One — Before You Apply, and After?**
    - Deadlines, links, who you emailed, where you stand, what they said.

* **Are You Updating Your Resume / Cover Letter for Each Application? How?**
    - If you tailor them, what do you change, and how long does it take?

* **What Do You Find Out Too Late?**
    - What are the things you want to be notified about, and when?

<br>

## Look Back at What You Just Wrote. That's Your Portal.

You didn't design software just yet. You described your own situation, and those are your requirements. What you build should flow naturally from them. Then you iterate, improving what you've built and adjusting it as conditions change.

<br>

## Step 02: Hand It to Claude

* **Open a Cowork session** connected to the project folder you made in Lab 00.

* Send Claude your answers along with this:

> We're a table of Yale students building an internship planner for ourselves. It should help us keep track of the internships we're applying to, remember deadlines and contacts, and stop finding things out too late. We'll build it step by step: a simple working version first, then we'll improve it.
>
> Here are our notes on how we track internship applications, and what goes wrong.
>
> [attach your photos, and add any other notes from your brainstorming]
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

<p class="info"><b>Hint:</b> Claude handles images and photos as input very well. Photograph your template, whiteboard and sticky notes with a phone and attach the pictures — handwriting, arrows, crossings-out and all. You don't need to type any of it out.</p>

<br>

## Step 03: Answer Its Questions, Then Judge the Mockup

* Claude will ask you a handful of questions. **Answer them as a table.**

* Then it shows you a mockup: a rough version with made-up data, before any real code exists.

* **Look at it properly.** Is this the thing you described? What's missing? What's there that nobody asked for?

* Say what's wrong and ask for another one. **Do not approve a mockup you don't like** — changing it now costs seconds, changing it after the build costs ten minutes.

<br>

## Step 04: Build It

* When the mockup is right, tell Claude to go ahead.

* Claude asks permission before it does things. Click **Allow**, or **Allow for this task** to reduce the clicking.

<br>

## Step 05: Take a Break

Builds take **ten minutes or more**, so this is a good time for a break.

* **Keep someone close.** Claude pauses to ask questions and waits until somebody answers. Nothing moves while it waits.

* **When you're back, talk about what comes next:**
    - What would you add or change first?
    - Who at your table would actually use this next week, and what would change the others' minds?

* **Compare with your neighbors.** The table next to you made different choices from the same questions.

<br>

## Step 06: Run It, Test It and Improve on It

* Claude will tell you how to start your app and give you a web address to open.

* **Add a few internships you'd actually go for.** Find the posting and paste the link.

* **What would you like to improve?** Did it do everything you asked for, or did it leave some things out?

* **What did you learn about this process that you'd like to keep?** Ask Claude to write those best practices and design principles into a Markdown file in your project folder. Congratulations, you have your first skills file!

* Next time you build something, ask Claude to read the skills file as part of the prompt.

<br>

## Step 07: Make It Do Something

Before you add anything, review the design. Does it look and work the way your table wants, or does it look like a default? A calendar view, a different layout or a different way of sorting might suit you better. Tell Claude what to change.

So far your app shows you things. Now make it act. Go back to what you wrote under "What Do You Find Out Too Late?" and choose one thing worth being told about.

### Every Table: Add a Send Reminder Button

* **Ask Claude to add the button.** Start from this, and change it to fit what your table wants:

> Add a "Send Reminder" button to our planner. When we click it, the portal's own code should connect to the workshop MCP server at the address below and use its reminder tool to send a reminder email or calendar invite about that internship to our table's lab account.

<p align="center" style="color:#800000"><b>[PLACEHOLDER - workshop MCP server address, access key and the name of its reminder tool]</b></p>
* **Check that it worked.** Click the button, then open the table leader's inbox. Did the message arrive, and is it what you asked for?

### Optional, If Your Table Is Ahead: Add a Chat Window

Now let your table type a request instead of clicking a button, using a small AI model running on the table leader's laptop.

* **Ask Claude to add the chat window.** Start from this:

> Add a small chat window to our planner, using the local Ollama model that's already installed. When we type a request such as "remind us about Goldman on Friday," send it to the model and have it fill in a fixed format, using Ollama's structured outputs: the action, the internship and the date. The portal's own code should then check that answer and carry it out, using the same reminder tool as the button. If the answer doesn't fit the format, show us a message and don't send anything.

<p align="center" style="color:#800000"><b>[PLACEHOLDER - name of the Ollama model, once chosen and tested]</b></p>
* **Try it, then try to break it.** Ask for something reasonable, then something strange. What does it do when it doesn't understand you?

* **Notice what you just built.** You type a request, and the system takes an action for you. A small model can handle a simple task like this without going to the cloud.

<br>

## Step 08: Make It Yours

Whatever time is left belongs to you. Go back to your brainstorming sheet and look at your portal honestly:

* **Did it hit everything?** What's on your sheet that isn't in the portal?

* **Is it easy to use?** Could someone at your table use it without help?

* **Would you really use it?** If not, what would change your mind?

Choose what matters most, ask Claude for it in your own words, then test it.

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

* **A thing that displays is a page. A thing that acts is an agent.** "What Do You Find Out Too Late?" is where yours crossed that line.

<br>

## Answer Sheet

*Use these if your table is stuck. Reading them first spoils the exercise.*

<p align="center" style="color:#800000"><b>[PLACEHOLDER - suggested prompts: a worked starting prompt, a prompt for adding the agentic action, and two recovery prompts for common failures]</b></p>
<br>

## What's Next

Your app lives in your project folder. Share it with your table, keep building, or start something else entirely — you now know how.
