# WebExtension: Crouching Tracker, Hidden Email

## Introduction
When a webpage shows a link with your email embedded as part of the link, it may be an attempt to track you.

This extension will change the cursor when you mouse over links containing the "@" symbol to give you an indication that you may be tracked and to proceed with caution.

This tactic has legitimate uses such as for email verification when signing up for new services, but it is also used by spammers or phishing emails that invite you to click on a link which then tells the server that your email address is active and even prefills your email in the webpage so that they look trustworthy.

### Example URLs:
- Absolute URL: [https://www.google.com/search?q=user@example.com](https://www.google.com/search?q=user@example.com)
- Protocol relative URL: [//www.google.com/search?q=user@example.com](//www.google.com/search?q=user@example.com)
- Relative URL: [/non-existent?q=user@example.com](/non-existent?q=user@example.com)
- Email links: [mailto:user@example.com](mailto:user@example.com)
