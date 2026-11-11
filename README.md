# Beach Camp RSVP

Mobile-friendly RSVP site with sunset artwork, 2 Truths, 1 Lie form, and private host dashboard.

## Enable GitHub Pages

In repository Settings → Pages, select Deploy from a branch, `main`, and `/(root)`. The public URL will be `https://jusrandtzn.github.io/reklamadorcamp/`.

## Configure live submissions

GitHub Pages is static hosting. To collect submissions and update the dashboard live, create a Firebase project, enable Realtime Database and Authentication (Anonymous plus Email/Password), create a host account, copy `firebase-config.example.js` to `firebase-config.js`, and add the project's Web app config. Use Database Rules to allow anonymous authenticated users to write submissions and reserve reads for password-authenticated hosts. Then publish `firebase-config.js`, open `dashboard.html`, and sign in as the host. See Firebase's Database rules for safe, field-specific validation.

The form stores name, three statements, selected lie, and timestamp. Lie selection is shown only on the dashboard. Without Firebase config, entries are stored only in the guest's browser.

Music starts when a visitor taps the player control because browsers restrict autoplay with sound. The sunset beach scene uses responsive CSS artwork.