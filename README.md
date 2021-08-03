# WebExtension: Crouching Tracker, Hidden Email ![appicon](https://raw.githubusercontent.com/em-te/webextension-crouching-tracker-hidden-email/main/icon_24.png)

## Introduction
When a webpage shows a link with your email embedded as part of the link, it may be an attempt to track you.

e.g. http://www.example.org/free_stuff?invite=user@example.com

This extension will change the cursor when you mouse over links containing the "@" symbol to give you an indication that you may be tracked and to proceed with caution.

This tactic has legitimate uses such as for email verification when signing up for new services, but it is also used by spammers or phishing emails that invite you to click on a link which then tells the server that your email address is active and even prefills your email in the webpage so that they look trustworthy.

## Details
This extension only works on absolute URLs because most trackers will redirect to another domain that is not within the control of the current website. This means relative URLs, FTP links and mailto links are not affected.

- Relative URL: [/non-existent?q=user@example.com](/non-existent?q=user@example.com)
- FTP link: [ftp://www.example.org/?q=user@example.com](ftp://www.example.org/?q=user@example.com)
- Email links: [mailto:user@example.com](mailto:user@example.com)

## Limitations
For maximum privacy, this extension achieves the task using pure CSS.

As a result, this extension will catch all URLs with the "@" symbol regardless of whether it conforms to a valid email syntax. For example "1@1" will be treated as an email address.

URLs which use the "@" symbol for stylistic purposes will also be treated like an email.

e.g. https://twitter.com/@Twitter/status/1390725076996268038

The author accepts this as an acceptable trade-off in exchange for guaranteed privacy.
