# Privacy Disclosure

**Extension:** Audible + Douban  
**Last updated:** November 22, 2026

Audible + Douban adds Douban book information to Audible book detail pages. This disclosure describes the extension's data handling based on its current source code.

## Information the extension processes

- **Audible book title:** The extension reads the title shown on an Audible `/pd/…` product page. It uses the title to search Douban Books and does not save it.
- **Douban book information:** It reads the matching book's title, author, rating, rating count, and up to five popular short comments so it can display them in the page panel. This information is held temporarily in memory while the page is open; the extension does not save it.
- **Douban session cookies:** Douban requests are made with the browser's existing cookies (`credentials: include`). The extension does not read, extract, or store cookie values. The browser may send applicable cookies to Douban with those requests, allowing Douban to recognize your session.

## How information is used and shared

The Audible title is sent to **Douban** as a book-search query. The extension then requests the matching Douban book page and its popular-comments page. Douban receives these requests, including applicable browser cookies, and handles them under its own privacy terms and practices. See [Douban's privacy policy](https://www.douban.com/about/privacy).

The extension does not send information to the extension developer or to any developer-operated server. It does not include analytics, advertising, or tracking code.

## Storage and retention

The extension does not use browser storage, local storage, or a remote database. It does not retain the title, Douban results, or cookies after the active page context is gone. Douban may process or retain request data according to its own policies.

## Permissions and access

The extension runs on Audible book product pages to read the book title and display its panel. It can access the specific Douban book-search and book-page URL patterns needed to make its lookups. It does not request broad browsing-history, tab, or cookie-management permissions.

## Your choices

You can disable or uninstall the extension in your browser's extension settings. You can also avoid using it while signed in to Douban; Douban may then show different results or require verification. Disabling the extension prevents its future lookups, though it does not control data Douban has already received.

## Changes and contact

This disclosure should be updated if the extension's data handling changes. For questions, contact the extension publisher through the contact channel provided on the extension's distribution page.

