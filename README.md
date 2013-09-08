Canonical Two-Factor Auth HTML5 client
=======================================

[Ubuntu One login](https://login.ubuntu.com), used for many Ubuntu and Canonical services (the Ubuntu wiki, Discourse, Ubuntu One itself, Launchpad, etc) has the option of allowing two-factor-auth. This is implemented using HOTP, a standard way to do this: when you log in, you go to your HOTP device and generate a new code, and then use that code along with your password to log in. There are many HOTP clients out there: Google Authenticator is a common one. It's nice to not have to rely on a native app, though, especially if that native app is not available for your platform.

Therefore, an HTML5 client-side app.

This is not specific to Ubuntu One login: this code is actually a completely generic JavaScript HOTP client for HTML5. It was written for Ubuntu One sign-in, though, so that's the language it uses.

It comes with an appcache, so if it's served over HTTP, it can be bookmarked as an "app" and will work offline. It contains no server components, so your HOTP keys are not used or even seen by the server.
