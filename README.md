# Contact Request

A one-file iPhone web app (`index.html`) for collecting **name, email and phone** from people you meet while networking. You don't install anything from the App Store, and you don't need a server or an account.

## Two ways to use it

| Mode | How it works | Where the contact ends up |
|---|---|---|
| **Tap / scan** (their phone) | They tap the NFC sticker on your phone case, or scan your QR code. The form opens on *their* phone. | When they submit, a pre-filled text (or email) to you opens. They hit **Send**. They can also save your contact card. |
| **Hand-over** (your phone) | You hand them your iPhone with the form open. | It's saved on your iPhone. From the ⚙︎ dashboard, tap **Add to Contacts** or export a CSV. |

> **Why an NFC sticker instead of phone-to-phone?** Apple doesn't let websites or third-party apps send data from one iPhone to another by tapping. The only built-in option is NameDrop, which swaps contact cards and can't show a custom form. A ~$1 NFC sticker on your case gives the same "tap phones" experience, and it works with any iPhone XS or newer and with most Android phones.

## Setup (about 10 minutes)

1. **Host the page (free) with GitHub Pages**: in this repo go to **Settings → Pages → Source: Deploy from a branch** and pick the branch and `/ (root)`. Your link will be like `https://<username>.github.io/Contact-Request/`.
2. **Open that link in Safari on your iPhone.** Tap Share → **Add to Home Screen**.
3. **Open the dashboard** by tapping ⚙︎ in the top-right corner. Fill in your name, headline, mobile number (and optionally your email) and the hosted link. Tap **Save**. A QR code and your share link appear.
4. **Make the tap sticker:** buy NTAG215 NFC stickers (Amazon, about $10 for 20). Install the free **NFC Tools** app, then go to *Write → Add a record → URL*, paste your share link, tap *Write* and hold the sticker near the top of your iPhone. Put the sticker on the back of your case.

Now when someone taps the back of your phone with theirs, a notification pops up, they open it, fill in the form and send you their details by text.

## Privacy

- Contacts collected in hand-over mode are stored only in Safari on your iPhone (local storage). Back them up by exporting the CSV now and then. Clearing Safari's website data erases them.
- Your name, number and email are in the share link (that's how the form knows where to send details). Only put in what you're happy to share with a new contact.
