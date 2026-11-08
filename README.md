# SafePaste — Day 12

Mask common private details in plain text before sharing a log, support request, or copied message. SafePaste processes the text in the browser and leaves it to you to review the output.

## Use it

Open `index.html` or visit the live demo. Paste text, select the detail types to find, and optionally add exact custom terms one per line. Select **Redact selected details**, review the result, then copy or download it.

## Features

- Detects common email addresses, phone-number formats, Luhn-valid card-number candidates, and IPv4 addresses.
- Finds several common API key and credential formats.
- Masks custom literal phrases without treating them as regular expressions.
- Shows how many matches were replaced by category without listing the original values.
- Copy or download the redacted text.
- Runs locally with no account, upload, storage, analytics, or external libraries.

## Privacy and limitations

Text remains in the current browser tab and is not uploaded or saved by the app. Pattern matching is best-effort: it may miss unusual formats or match ordinary numbers. Card numbers are filtered with a checksum, but that does not prove a number is an active card. Review the output manually and add names, IDs, addresses, or other sensitive details to the custom list before sharing.

## GitHub Pages

This is a static single-file app. GitHub Pages can serve it from the repository's `main` branch and root folder.

## Built with

HTML, CSS, and browser JavaScript. MIT License.
