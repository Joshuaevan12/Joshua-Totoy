# Google Sites Single Embed Instructions

Using file:

- `government-sheet-embed.html`

## How to use in Google Sites

1. Host `government-sheet-embed.html` on one public domain.
2. In Google Sites, go to **Insert > Embed > By URL**.
3. Paste your hosted URL.

Example:

```text
https://your-domain/government-sheet-embed.html
```

## Recommended URL Parameters

Base:

```text
https://your-domain/government-sheet-embed.html
```

With near real-time refresh:

```text
https://your-domain/government-sheet-embed.html?live=true&refreshSeconds=5
```

Open a specific page:

```text
https://your-domain/government-sheet-embed.html?sheet=Incoming%20%26%20Outgoing%20Docs&live=true&refreshSeconds=5
```

Force a specific header row if needed:

```text
https://your-domain/government-sheet-embed.html?sheet=Incoming%20%26%20Outgoing%20Docs&headerRow=2
```

## If you need iframe format

```html
<iframe src="https://your-domain/government-sheet-embed.html" width="100%" height="980" style="border:0;" loading="lazy"></iframe>
```

## Notes

- This setup now uses one file only: `government-sheet-embed.html`.
- Make sure your Google Sheet is shared publicly (or published to web) so fetch requests can work.
- For best compatibility, use **Insert > Embed > By URL** in Google Sites.
