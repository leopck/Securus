# What is Securus?

An open source implementation of a secured methodology to sign-in to any system/website without the need to key in password. Passwords are challenges.

Without the need to be tied down to Google, FB or other social media which becomes a target.

Even if the Securus is comprimised, its' database cannot be used without the Enigma key because the key changes every 12 hours. Or if compromised is known, immediate change to the key is activated.

# Reference design

1. Enigma design
2. OAuth

## Long term goal

Get other websites to implement this feature. This way every website will constantly change password and there'll be no fix password moving forward. Even if the database is hacked, but because the website is constantly changing and the website doesn't have the key to unlock then even if the password got hack but without the key, it's not possible to snatch it.

Another possible goal is to have a "Sign-up with Securus" similar to "Sign-up with Google"
then "Sign-in with Securus"

This will automatically select the most secure manner to sign in without the concern of security.
