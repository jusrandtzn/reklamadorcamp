# Beach Camp RSVP

Mobile-friendly RSVP site with a sunset beach scene, animated floaties, 2 Truths, 1 Lie form, and a live host dashboard.

## Public site

- RSVP: https://jusrandtzn.github.io/reklamadorcamp/
- Host dashboard: https://jusrandtzn.github.io/reklamadorcamp/dashboard.html
- Themed QR card: https://jusrandtzn.github.io/reklamadorcamp/qr.html

## Firebase setup already connected

The site uses the `Beach Camp RSVP` Firebase project and its Realtime Database. The Firebase browser config is in `firebase-config.js`; Firebase Web config/API keys are public identifiers, not server secrets. Database Rules—not secrecy of the web config—protect submissions.

Guests sign in anonymously before submitting. Database rules allow an anonymous guest to create one validated submission and prevent updates. Reads require a password sign-in using the verified host email. The personal email appears only in Firebase Database Rules, not in the public repository. Authentication also authorizes `jusrandtzn.github.io`.

## Create your host login

1. Open the host dashboard above.
2. Select **Create one** below the sign-in form. Use your personal Firebase email, choose a password yourself, and create the account.
3. Open the Firebase verification email, follow its link, return to the dashboard, then choose **I verified — check again**.
4. Sign in with that email/password whenever you want to review live submissions.

Only the verified host email can read the submissions. Guest data includes name, three statements, lie selection, and submission time. Keep the dashboard and guest responses private.

## Music

“Vacation” by Dirty Heads loads after a visitor taps the music control because browsers commonly block audible autoplay.
