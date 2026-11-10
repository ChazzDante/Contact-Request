# Connect

A minimalist, one-file iPhone web app (`index.html`) for collecting **name, email and phone** from people you meet while networking. Show your QR code; they scan it with their camera and their details come straight to you. You don't need an App Store app, a server or an account.

## How it works

- **My code**: your personal QR code, showing your name and headline. Someone scans it with their iPhone or Android camera and a short form opens on *their* phone.
- **They fill in the form**, tap Continue, then **Send by text**. A message to you with their details opens already filled in; they just hit Send. They can also save your contact card.
- **Hand over**: if their camera isn't handy, hand them your phone. Their details are saved on your iPhone, and **Done** (top right) takes you back.
- **Contacts**: everyone collected on your phone. Add them to iPhone Contacts one at a time or all at once, text them, or **Export** a spreadsheet (CSV).
- **Profile**: your name, headline, mobile number and optional email.

The QR generator is built into the file, so your code still shows when signal at an event is weak.

## Setup (about 5 minutes)

1. **Host the page for free with GitHub Pages**: in this repo go to **Settings → Pages → Source: Deploy from a branch**, then pick the branch and `/ (root)`. Your link will be like `https://<username>.github.io/Contact-Request/`.
2. **Open that link in Safari on your iPhone**, then tap Share → **Add to Home Screen**.
3. Fill in your profile and tap **Save**. Your QR code appears.

## Privacy

- Contacts collected with Hand over are stored only in Safari on your iPhone (local storage). Back them up now and then with Export. Clearing Safari's website data erases them.
- Your name, headline, number and email are part of the QR link (that's how the form knows where to send details). Only include what you're happy to share with a new contact.

QR generation uses [qrcode-generator](https://github.com/kazuhikoarase/qrcode-generator) by Kazuhiko Arase (MIT License), included inline.
