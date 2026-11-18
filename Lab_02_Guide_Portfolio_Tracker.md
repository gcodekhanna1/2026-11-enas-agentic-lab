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
- ENAS NOTE: one document. The discovery questions and the build steps live together here. Lab 01 is the model: keep the two guides parallel.
- ENAS NOTE: students write their own prompt. Need a Nudge? links to Lab_02_Prompt_Ideas, a rescue rope, not the path (renamed from Answer Sheet 11/17).
- ENAS NOTE: stocks and investments only — no budget variant. Tracking and explaining only: no buy/sell advice, no real brokerage connection.
-->

# Lab 02 — Stock and Investments Tracker

*Thirty minutes describing the problem. The rest of the session building the answer.*

## The Goal

Maybe you've just put your first few hundred dollars into the market, or you follow a handful of companies you care about. Either way, the prices move every day, the headlines never stop, and it's hard to tell what actually matters — or why anything moved at all.

You want one place that shows how your investments are doing, and explains what changed and why.

* ⚠️ **This is a tracking and explaining tool, not an advice tool.** It doesn't tell anyone what to buy or sell, and it never connects to a real brokerage account or real money.

<br>

## Step 01: Brainstorming and Discovery

*About 30 minutes, as a guide rather than a limit.*

Work as a team to discuss the questions below. Feel free to add some of your own — these are just starters.

Remember that we are building and iterating. As a group, use your judgment for when you have done enough discovery to move on to building.

Capture your answers on your Planning & Discovery Worksheet, whiteboard and sticky notes. You'll photograph them and hand them to Claude at the end.

* **Who Is This For?**
    - A student with their first few hundred dollars invested, a parent, a campus investment club? Pick one person and keep them in mind.

* **How Do You Follow Investments Today?**
    - A brokerage app, news alerts, a group chat, social media, not at all? What works, and what's annoying?

* **When a Price Moves, What Do You Wish You Understood?**
    - Why did it move? Is it a big move for this company, or a normal day? Did anything happen in the news?

* **What Should It Warn You About?**
    - A big drop, too much of your money in one company, news about something you own? When would you want to hear about it?

* **What Would You Never Want It to Do?**
    - Where's the line between a tool that explains and a tool that tells you what to do? Write down two things it must not do.

* **What Should It Look Like When You Open It?**
    - One big number, a list, a chart, a short summary of the day? Sketch it.

<br>

## Look Back at What You Just Wrote. That's Your Portal.

You didn't design software just yet. You described your own situation, and those are your requirements. What you build should flow naturally from them. Then you iterate, improving what you've built and adjusting it as conditions change.

<br>

## Step 02: Hand It to Claude

* **Open a Cowork session** connected to the project folder you made in Lab 00.

* Send Claude your answers along with the prompt below. It asks for a *minimum viable product*: the simplest version that actually works, which you'll improve from there.

<p class="info"><b>Hint:</b> Claude handles images and photos as input very well. Photograph your worksheet, whiteboard and sticky notes with a phone and attach the pictures — handwriting, arrows, crossings-out and all. You don't need to type any of it out.</p>

> We're a table of Yale students building a stock and investments tracker for ourselves. It should show how a set of investments is doing, and explain what changed and why, in plain language. It's for tracking and explaining only: it must never tell us what to buy or sell, and it never connects to a real brokerage account. We'll build it step by step: a simple working version first, then we'll improve it.
>
> Here are our notes on how we follow investments today, and what we wish we understood.
>
> [Paste your notes from the brainstorming worksheet here. If you have photos of sticky notes, the whiteboard or sketches, attach them as well.]
>
> Build us an initial minimum viable product that we can further customize working with you.
>
> Build it with:
> - Streamlit, in Python. Please don't use a different framework.
> - uv to install whatever it needs.
> - One start file, so we can run it again later with a single command.
> - Sample data so we can see it working right away: about seven well-known stocks, such as Apple (AAPL), Tesla (TSLA), Nvidia (NVDA) and Microsoft (MSFT), with made-up prices and headlines clearly labelled as sample data. Let us keep, remove or add stocks. We'll connect it to live market data later.
>
> Before you build anything: ask us up to five questions about whatever is unclear, then show us a mockup using sample data. Wait for us to approve the mockup before you write the real thing.

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
    - Your portal will explain *why* something moved. How would you know if that explanation were wrong?
    - Where's the line between explaining and advising, and why does it matter for a tool like this?

* **Compare with your neighbors.** The table next to you made different choices from the same questions.

<br>

## Step 06: Run It, Test It and Improve on It

* Claude will tell you how to start your app and give you a web address to open.
* **Don't see a change you asked for?** When Claude says it's done, check that it restarted the portal (ask it to if it didn't), then refresh your browser page. A refresh on its own isn't always enough.

* **Make the list your own.** Remove stocks you don't care about and add the ones you do. The prices are still made up; you'll make them live in Step 07.

* **Use it as your person would.** Can you tell, at a glance, how the investments are doing today?

* **What would you like to improve?** Did it do everything you asked for, or did it leave some things out?

* **What did you learn about this process that you'd like to keep?** Ask Claude to write those best practices and design principles into a Markdown file in your project folder. Congratulations, you have your first skills file!

* Next time you build something, ask Claude to read the skills file as part of the prompt.

* **Step back and look at what you've built.** Does it look and work the way your table wants, or like a default? What else would you like in it: a chart, a different layout, sorting, a summary at the top? Ask Claude for it, then test it.

<br>

## Step 07: Make It Live, Then Make It Do Something

So far, your portal shows you made-up prices. Now it's time to connect it to the market, and have it act on what it finds.

Remember MCP, the "USB-C port" for AI? We built an MCP server for this class, so your portal has tools it can use. For this lab, it serves:

* **Live market quotes:** real prices for real stocks, such as Apple or Nvidia. Market data services usually charge for this; the workshop server fetches the quotes from one on the whole class's behalf and shares them, so your table doesn't need its own paid subscription. The 100 largest companies in the S&P 500 are ready before class starts; any other stock is fetched the first time someone asks for it.
* **A mock portfolio:** seven made-up companies, with prices, price history and news that line up with the price moves, so a portal can explain *why* something moved. Useful for trying ideas the live market can't give you on demand.

The server lives at `https://mcp.paradigmventures.ai/mcp`. [See how it fits together](Lab_02_How_It_Works.html).

### Make It Live

* **Ask Claude to swap your made-up prices for live ones.** Start from this, and change it to fit what your table wants:

> Connect our tracker to the workshop MCP server at https://mcp.paradigmventures.ai/mcp, and replace our made-up prices with live ones from its get_live_quote tool, for every stock on our list. Keep our list as it is, and keep letting us add and remove stocks.
>
> - Our table's lab account is demo-XX@paradigmventures.ai. Pass it as the `table` value on every call, so the workshop staff can see which table is calling.
> - The server's access key is: `LCpM2l-L1_Vd1wybj5KPHovFDYNmKq5y`. Keep it in a local settings file, not in the code.
> - Use the current official MCP Python library (`mcp`), and check how its current version works rather than relying on memory.
> - The quotes are shared by the whole class: fetch them when the page loads and when we press a Refresh button, at most once a minute, never in a loop.
> - If a quote comes back marked stale, show that it's the last known price. If the server says it's busy, show that message and let us try again.
> - Keep it simple: a first version we can try within a few minutes. We'll tell you what to improve.

* **Check that it worked.** Make sure Claude restarted the portal (if it doesn't tell you, ask it how). Then refresh your browser page. Do the prices match what you'd see in a news app? Add a stock that isn't on your list yet, and watch it appear.

* **Good to know: live quotes come with prices, not news.** Explaining a real move is a hard problem, and a good one to talk about: where would your portal get the reason?

### Suggestion: Make It Warn You

A tracker that only shows numbers waits for you to notice things. One that warns you does the noticing for you. You may already have this under "What Should It Warn You About?"

* **Ask Claude for the warning your table wants.** For example, if your portal knows how many shares you own, a warning when too much of your money sits in one company:

> Add a warning to our tracker when any one stock is more than 25% of our portfolio's value, using the live prices and the number of shares we entered. Show it at the top of the page, in plain words: which company, what share of the portfolio it is, and why that matters. Let us change the 25% from the page.
>
> - Don't tell us what to buy or sell. Explain the risk; we decide.

* **Want the warning in your inbox?** The workshop server can also email your table's lab account, the same tool Lab 01 uses (`send_reminder`). Ask Claude to add an **Email This Warning** button, and tell it not to send real emails while it tests. You'll send the first one yourselves from the portal.

### Suggestion: Explain Why, with the Mock Portfolio

The mock portfolio is seven made-up companies whose news explains every price move, so you can build the "why did it move?" feature now and see it work.

* **Ask Claude to add a Mock Portfolio page:**

> Add a Mock Portfolio page to our tracker, using the workshop server's mock portfolio data: get_holdings for the portfolio, get_prices for the day's prices, get_price_history for charts and get_news for the headlines. Use the same server address, lab account (as `table`) and access key as before. For the biggest price moves today and over the past week, show the headline that explains each one beside the move, in one sentence. If there's no matching headline, say so rather than guessing.

* **Try it, then question it.** Pick one explanation and check it against the news yourselves. Is it right? How would you know if it weren't? And look at how the portfolio is split: does anything deserve a warning?

### Suggestion: Add a Chat Window

Adding a chat window lets your table ask about your stocks in plain English, using a small AI model running on the table leader's laptop.

* **Ask Claude to add the chat window.** Start from this:

> Add a small chat window to our tracker, using the local Ollama model that's already installed. When we type a question such as "how is Nvidia doing today?", send it to the model and have it fill in a fixed format, using Ollama's structured outputs: the kind of question (how it's doing, how it moved, or how much of the portfolio it is) and the stock. The portal's own code should then check that answer, get the facts from the workshop server and show them. If the answer doesn't fit the format, show us a message instead.
>
> - Use the qwen3.5:4b model, with its thinking turned off (think: false), so replies come back quickly.
> - Use the same workshop server address, lab account and access key as above, or ask us for them if we haven't given them to you yet.
> - Don't install Ollama or download the model in your own workspace to test it. You can't reach the one on our laptop from there. Write the code, test the checking with a few sample answers, and we'll try it with the real model when we run the portal.
> - Make the chat window easy to find: put it near the top of the sidebar, with a clear heading and a text box a few lines tall.
> - The portal must never tell us to buy or sell. If we ask for advice, it should say it only explains.
> - Keep it simple: a first version we can try within a few minutes. We'll tell you what to improve.

The model, `qwen3.5:4b`, is the one your table leader installed in Lab 00.

* **Restart and refresh.** As before, make sure Claude restarted the portal (if it doesn't tell you, ask it how), then refresh your browser page.
* **Try it, then try to break it.** Ask something reasonable, then something strange. Ask it which stock to buy. What does it do?

* **Notice what you just built.** Your portal goes and gets facts from another system, decides whether something deserves a warning, and tells you without being asked. A thing that only displays is a page; a thing that acts is an agent.

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

* **Live quotes say "busy" or "stale":** the whole class shares them. Wait a minute and press Refresh.

* **You're out of ideas:** see **Need a Nudge?** at the bottom.

<br>

## Key Takeaways

* **The thirty minutes of talking did more for your build than any single prompt.** You described a problem; the design came out of the description.

* **You reviewed a plan before accepting the work.** That one habit separates people who get good results from people who get impressive-looking ones that break.

* **You directed an agent.** It asked, planned, used tools and built — you decided what mattered. And your skills file means the next build starts from what you learned.

* **A thing that displays is a page. A thing that acts is an agent.** Going live, the warning and the explanation are where your tracker crossed that line.

* **An explanation produced by a model is a claim, not a fact.** Knowing how you'd check it is part of building responsibly.

<br>

## Need a Nudge?

*Try your own prompts first. They're what make the portal yours.*

If your table is stuck, here are [a few prompts other tables have tried](Lab_02_Prompt_Ideas.html). Borrow an idea, then put it in your own words.

<br>

## What's Next

Your app lives in your project folder. Share it with your table, keep building, or start something else entirely — you now know how.
