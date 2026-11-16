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
- ENAS NOTE: a side page for Lab 02 Step 07, matching Lab_01_How_It_Works. Linked from Step 07, not listed on the landing page.
-->

# Lab 02 — How It Fits Together

*What happens when your tracker gets its prices and news.*

<br>
<p align="center">
  <img src="Lab_02_How_It_Works_Diagram.svg" alt="On the table leader's laptop, the portal's code asks for data when the page loads or when you press Refresh, or after a small local model turns a typed question into a fixed format. The request goes over the internet, with the access key, to the workshop MCP server. For real stocks its get_live_quote tool serves prices from a shared cache, fetching from a market data service about once a minute for the whole class. For the mock portfolio its own tools serve seven made-up companies whose news explains their moves. Its send_reminder tool can email a warning to the table's lab account. The data comes back to the portal, which decides what to show." width="100%">
</p>
<br>

## What Happens When Your Tracker Refreshes

* **Your portal asks:** when the page loads or you press **Refresh**, your portal's code sends a request over the internet to the workshop MCP server, with the access key and your table's lab account.

* **Real stocks:** the server's `get_live_quote` tool looks in its shared cache. If a price is less than about a minute old, it answers straight away. If not, it fetches a fresh one from a market data service, once for the whole class.

* **The mock portfolio:** the server's own tools (`get_holdings`, `get_prices`, `get_price_history`, `get_news`) serve seven made-up companies whose news lines up with their price moves.

* **Your portal decides:** the answers come back, and your portal's own code decides what to show — the prices, a warning if one stock is too big a share, the headline that explains a move.

<br>

## Why One Shared Connection?

Market data services charge for live prices and limit how many you can ask for each minute. Instead of every table signing up, the workshop server holds one connection and shares it. Each price is fetched once and served to every table that asks, so the whole class stays well within the limit.

That's also why the guide asks you to refresh at most once a minute. If the server says it's busy, wait a minute and try again. A price marked stale is the last one the server had.

<br>

## The Chat Window and the Emailed Warning

* **The chat window (optional):** you type a question in plain English. The small Qwen model on the laptop turns it into a fixed format — the kind of question and the stock — and your portal's code checks it, then asks the server for the facts. What you type doesn't go to the cloud.

* **The emailed warning (optional):** the server's `send_reminder` tool, the same one Lab 01 uses, emails your table's lab account, which forwards it to the table leader's inbox.

<br>

## Where's Claude?

Claude built your tracker, but it isn't in this loop. Once it's built, your portal does the asking, the checking and the warning. That's the difference between a tool that helps you build something and the thing you built doing work on its own.

<br>

[← Back to Lab 02, Step 07](Lab_02_Guide_Portfolio_Tracker.html)
