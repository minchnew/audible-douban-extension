# Audible + Douban

A local Chrome Manifest V3 extension that adds a small Douban book information panel to Audible book detail pages.

## What it does

1. Runs on Audible `/pd/…` product pages.
2. Reads the product title from the page.
3. Searches Douban Books (`cat=1001`) and opens the strongest title match.
4. Reads the rating and up to five short comments from the Douban book page.
5. Shows the result in a panel on the Audible page, with a link to the Douban entry.

The extension sends the Audible book title as a search query to Douban and includes your existing Douban cookies on requests to `search.douban.com` and `book.douban.com` so Douban can recognize your session. The extension does not read or store those cookies. Douban may still require verification; if so, the panel links to the Douban search page and lets you retry after completing any check there.

## Load it in Chrome

1. Open `chrome://extensions`.
2. Turn on **Developer mode**.
3. Choose **Load unpacked** and select this directory.
4. Open or reload an Audible book detail page.

No build step or external libraries are required. Douban's page markup can change, so its search parsing and comment selectors may need updates in the future.
